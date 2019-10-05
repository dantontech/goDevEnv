# goDevEnv
A Go Development environment in a container

## Usage

### Step 1:
Clone this repository on a server with Docker.

### Step 2:
Build the container:
```
sudo docker build -t danton.tech/godevenv .
```

### Step 3:
Run the container:
```
sudo docker run --name=goDevEnv -v /home/danton/.ssh/:/home/danton/.ssh/ -p 3000:3000 -it danton.tech/godevenv
```

### Step 4:
Once inside the container, launch Neovim.
```
nvim
```

### Step 5:
Run GoInstallBinaries to complete vim-go setup
```
:GoInstallBinaries
```


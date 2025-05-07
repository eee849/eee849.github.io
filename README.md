# Unblocked-Browser/OS SERVER 
This is a fully functional server-side docker vnc that works currently without audio.

# Installation and Requirements
It is recommended you download the files once I make a new release and put them on a codespace and then run these two commands once extracted and in void linux directory.

```bash
docker build -t void-desktop .
```

Once built, the run command is:

```bash
docker run -it --rm \
  --shm-size=1g \
  -p 6080:6080 \
  --name void-desktop \
  void-desktop
```

# How do I access the VNC/Graphical Display?
If you are in codespaces, you go to ports and click on the link for port 6080.

If you are running this on actual server technology, port forward and then navigate to the link given by the server (if you arent and want to use on your home network with server technology, just type localhost://6800 after starting the VNC.

#### Build
```bash
docker build -t one2rist/ubuntu_dev:0.2 .
```

#### Images
```bash
docker images --all
```

#### Tag
```bash
docker tag one2rist/ubuntu_dev:0.2 one2rist/ubuntu_dev:0.3 
# tag source -> target
```

#### Push
```bash
docker push one2rist/ubuntu_dev:0.2
```

#### Run
```bash
docker run -it one2rist/ubuntu_dev:0.2
# -i, --interactive                    Keep STDIN open even if not attached
# -t, --tty                            Allocate a pseudo-TTY
```

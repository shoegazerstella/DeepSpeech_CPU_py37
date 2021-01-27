# DeepSpeech CPU on python 3.7
This version of [PaddlePaddle DeepSpeech](https://github.com/PaddlePaddle/DeepSpeech) is intended for inference only to run on CPU with python 3.7

### Docker usage
```
docker build -f Dockerfile_cpu_py37 -t deepspeech-cpu .
docker run -v /your/data/and/model/dir/:/root/DeepSpeech/DATA/ -it deepspeech-cpu
```

make sure to use the flag `--use_gpu=False` when calling `infer.py`

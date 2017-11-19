# Codenvy Training:

## Performance
SSE4.1 SSE4.2 AVX AVX2 FMA  
[Tensorflow-1.4.0](https://github.com/EN10/BuildTF/raw/771df48529285c69ef760327121e996750b3916e/tensorflow-1.4.0-cp27-none-linux_x86_64.whl)

## Requires:
Copy /tmp files:

    cp /projects/Speech/train/speech_dataset /tmp/speech_dataset -r
    cp /projects/Speech/train/speech_commands_train /tmp/speech_commands_train -r
    cp /projects/Speech/train/retrain_logs /tmp/retrain_logs -r

## Training:
    python train/train.py --start_checkpoint=/tmp/speech_commands_train/conv.ckpt-100

Update /tmp files:

    cp /tmp/speech_commands_train /projects/Speech/train/ -r
    cp /tmp/retrain_logs /projects/Speech/train/ -r

## speech_dataset
    cp Speech/train/speech_dataset/speech_commands_v0.01.tar.gz /tmp/speech_dataset/speech_commands_v0.01.tar.gz
    ls /tmp/speech_dataset/

LICENSE             bed   dog    five  happy  marvin  off  right   six                           testing_list.txt  two                  wow
README.md           bird  down   four  house  nine    on   seven   speech_commands_v0.01.tar.gz  three             up                   yes
_background_noise_  cat   eight  go    left   no      one  sheila  stop                          tree              validation_list.txt  zero
# AI Vintage Robot Identifier

Uses imagenet to identify a robot using an imagenet model.
Currently can only recognize Robot Commander II,II, Pathfinder, Robot 2001 but dataset can be added to

# Usage

run the docker container
run the commands:
ET=models/robots
DATASET=data/robots

run:
imagenet.py --model=$NET/resnet18.onnx --input_blob=input_0 --output_blob=output_0 --labels=$DATASET/labels.txt $DATASET/test/pathfinder/01.jpg pathfindertest.jpg

"$DATASET/test/pathfinder/01.jpg" can be replaced with the directory of your test image

Script will output it's identification after about a minute.

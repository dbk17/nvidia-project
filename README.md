# AI Vintage Robot Identifier

Uses imagenet to identify a robot using an imagenet model.

# Usage

run the docker container
run the commands:
ET=models/robots
DATASET=data/robots

imagenet.py --model=$NET/resnet18.onnx --input_blob=input_0 --output_blob=output_0 --labels=$DATASET/labels.txt $DATASET/test/pathfinder/01.jpg pathfindertest.jpg

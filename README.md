
# ZEP experiment: Inference
Five images and text is shown. The participant is to make a choice and select one of the corner images.

Trials start by pressing SPACE. Selection of the images can be done via either a 4-buttoned response box or the Numpad keys 4, 5, 1 and 2 for top left, top right, botton left and bottom right respectively.

The image of choice will highlight for a short while.

Eyetracking is possible but turned off by default. To turn on make sure the correct booleans are set in the test_items and defs: USE_EYETRACKING.

# AUTHOR(s)
* Chris van Run (C.P.A.vanrun@uu.nl)
* Rianne Vlaar (M.A.J.Vlaar@students.uu.nl)

# Groups
There are four possible groups (GRP1..GRP4). These have no effect other than to support participant categorization.

# Audio
Original script allowed the playback of audio. This has been indirectly disabled by leaving the audio filename input for the stimuli empty.

# Customisation
You can change the content of the stimuli by editing the .csv files in `stimuli` directory. For ease of editing the stimuli files are specified in different files for each of the types: A, B or C.

Images size, location and scaling can be adjuste via the following values in `modules/defs.zm`:
    TEST_CANVAS_SIZES_WIDTH = 400;
    TEST_CANVAS_SIZES_HEIGHT = 400;
    DISTANCE_OUTER_PICTURES = 300;
    IMAGE_SCALING = 0.5; //Liefst op 1.0

Texts (instructions and buttons) can be edited by changing the line `import text_nl.zm` to `import text_en.zm` in `infer.zm`. One can edit the content of the text variables in `modules/texts_*.zm`.

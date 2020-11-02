# Dataset-TacAct
Last updated: 2020-10-19
------------------------------------------------------------------------------------------------------------------------

General description

	TacAct, is a collection containing 24000 gesture captures of 12 different Human-Robot touch gestures. 
	The gestures were performed in right and left hand, on a pressure sensor grid wrapped around a mannequin arm. 

	This dataset was collected by Peng W, Dicai Chen, Hebei University of Technology.  

Data recording

	Data was recorded October 2020.
	Recorded gesture captures: 12 gestures * 40 repetitions * 50 subjects = 24000 touch gestures in total

Data structure 

	File: subject_gesture_variant_repeat number.xlsx
	Attributes:
		#1. subject - subject number (domain: 1-50)
		#2. gesture - gesture label (domain: 1-12): 
			1 = pull, 
			2 = squeeze, 
			3 = push, 
			4 = hold, 
			5 = grasp, 
			6 = poke, 
			7 = static drag, 
			8 = strongly hit, 
			9 = soft slide, 
			10 = scratch,
			11 = soft hit (twice), 
			12 = sliding drag,
                #3. variant - right hand or left hand (domain: R,L):  
                         R = right hand
                         L = left hand
                #4. repeat number - number of repetitions of the actions (domain: 1- 20)

Data format: The pressure indexes are arranged in the form of 32*32 matrices

		Mapping of matrix to physical sensor grid as wrapped around the mannequin arm, matrix 32*32 are facing the participant:
		  1	   2    3	   4	  5	 ...   32
		 33	  34   35	  36	 37	 ...   64
		 65	  66   67	  68	 69	 ...   96
		 97	  98   99	 100	101	 ...  128
		  .	   .    .	   .	  .	        .
		  .	   .    .	   .	  .	        .
		  .	   .    .	   .	  .	        .
		993	 994  995	 996	997	 ... 1024
		  
------------------------------------------------------------------------------------------------------------------------

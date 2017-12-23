# rhyming-dictionary
Rhyming dictionary based on the "CMU Pronouncing Dictionary", a reverse phoneme rhyming dictionary. 

A single file includes dictionary. It may be used as an EC2 Lamda fuction without accessing records with slight mod for lambda.

The original dictionary can be found here. http://www.speech.cs.cmu.edu/cgi-bin/cmudict

Search for a word or similar sounding word. 


var dict = require('rhyming_dictionary');
console.log(dict.lookup(process.argv[2]));


Command line example: $ node rdict.js schoepf

[ 'schoepe',
  'schoepf',
  'schoepp',
  'shope',
  'dope',
  'hope',
  'proctoscope',
  'kaleidoscope',
  'laryngoscope',
  'bronchoscope',
  'telescope',
  'oscilloscope',
  'ophthalmoscope',
  'horoscope',
  'gyroscope',
  'polariscope',
  'periscope',
  'stereomicroscope',
  'microscope',
  'antroscope',
  'gastroscope',
  'stethoscope',
  'worldscope',
  'interscope',
  'endoscope',
  'marketscope',
  'scope',
  'cope',
  'koep',
  'koepp',
  'koeppe',
  'kope',
  'cantaloupe',
  'antelope',
  'envelope',
  'elope',
  'slope',
  'lope',
  'mope',
  'partenope',
  'knope',
  'nope',
  'pope',
  'groep',
  'grope',
  'heliotrope',
  'allotrope',
  'tightrope',
  'isentrope',
  'strope',
  'misanthrope',
  'rope',
  'softsoap',
  'soap',
  'sope',
  'isotope',
  'epitope',
  'tope',
  'swope' ]


Based on this phone list below. Therefore, "abhorrence AH.B.HH.AO.R.AH.N.S" ends in an 'S', and 'abolishes AH.B.AA.L.IH.SH.IH.Z' ends in 'Z'. 

        Phoneme Example Translation
        ------- ------- -----------
        AA	odd     AA D
        AE	at	AE T
        AH	hut	HH AH T
        AO	ought	AO T
        AW	cow	K AW
        AY	hide	HH AY D
        B 	be	B IY
        CH	cheese	CH IY Z
        D 	dee	D IY
        DH	thee	DH IY
        EH	Ed	EH D
        ER	hurt	HH ER T
        EY	ate	EY T
        F 	fee	F IY
        G 	green	G R IY N
        HH	he	HH IY
        IH	it	IH T
        IY	eat	IY T
        JH	gee	JH IY
        K 	key	K IY
        L 	lee	L IY
        M 	me	M IY
        N 	knee	N IY
        NG	ping	P IH NG
        OW	oat	OW T
        OY	toy	T OY
        P 	pee	P IY
        R 	read	R IY D
        S 	sea	S IY
        SH	she	SH IY
        T 	tea	T IY
        TH	theta	TH EY T AH
        UH	hood	HH UH D
        UW	two	T UW
        V 	vee	V IY
        W 	we	W IY
        Y 	yield	Y IY L D
        Z 	zee	Z IY
        ZH	seizure	S IY ZH ER

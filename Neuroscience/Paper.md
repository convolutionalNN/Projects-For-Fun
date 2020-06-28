1‌ ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
A‌ ‌Novel‌ ‌Approach‌ ‌to‌ ‌Biologically-Modeled‌ ‌
Neural‌ ‌Connectivity‌ ‌and‌ ‌Neuroplasticity‌ ‌in‌ ‌
Artificial‌ ‌Neural‌ ‌Networks‌ ‌
 ‌
 ‌
 ‌
Word‌ ‌Count:‌ ‌~5480‌ ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
2‌ ‌
Table‌ ‌of‌ ‌Contents‌                                                                                          ‌Page‌ ‌
Literature‌ ‌Review………………………………………………………………………..3‌ ‌
‌Introduction………………………………………………………………....……3‌ ‌
‌A‌ ‌Brief‌ ‌Overview‌ ‌of‌ ‌Neuroscience…………………………………………….4‌ ‌
Origins...………………………………………………………………….4‌ ‌
Plasticity...………………………………………………………………..8‌ ‌
A‌ ‌Brief‌ ‌Overview‌ ‌of‌ ‌Artificial‌ ‌Intelligence…………………………………….11‌ ‌
Origins...………………………………………………………………...11‌ ‌
Existing‌ ‌Optimization‌ ‌Success...……………………………………..13‌ ‌
‌Existing‌ ‌Artificial‌ ‌Neural‌ ‌Connectivity‌ ‌and‌ ‌Neuroplasticity………………...14‌ ‌
Conclusion...……………………………………………………………….......18‌ ‌
Methodology...………………………………………………………………………….19‌ ‌
Experimental‌ ‌Design...………………………………………………………..19‌ ‌
Machine‌ ‌Learning‌ ‌Theory‌ ‌and‌ ‌Mathematics...……………………………..21‌ ‌
Justification‌ ‌of‌ ‌Method………………………………………………………..24‌ ‌
Biologically-Derived‌ ‌Equations‌ ‌and‌ ‌Implementation……………………….‌ ‌
Results‌ ‌and‌ ‌Analysis...………………………………………………………...‌ ‌
Limitations...…………………………………………………………………….‌ ‌
‌Conclusions‌ ‌and‌ ‌Future‌ ‌Directions...………………………………………...‌ ‌
References……………………………………………………………………………...‌ ‌
Appendix‌ ‌I……………………………………………………………………………….‌ ‌
‌Appendix‌ ‌II……………………………………………………………………………....‌ ‌
3‌ ‌
Literature‌ ‌Review‌ ‌
Introduction‌ ‌
You‌ ‌are‌ ‌using‌ ‌it‌ ‌when‌ ‌you‌ ‌purchase‌ ‌an‌ ‌Uber,‌ ‌talk‌ ‌to‌ ‌Siri,‌ ‌and‌ ‌scroll‌ ‌through‌ ‌ ‌
Amazon‌ ‌recommendations:‌ ‌it’s‌ ‌artificial‌ ‌intelligence.‌ ‌“Artificial‌ ‌Intelligence‌ ‌is‌ ‌probably‌ ‌
the‌ ‌most‌ ‌important‌ ‌thing‌ ‌humanity…has‌ ‌ever‌ ‌worked‌ ‌on.‌ ‌More‌ ‌profound‌ ‌than‌ ‌electricity‌ ‌
or‌ ‌fire”.‌ ‌This‌ ‌quote‌ ‌from‌ ‌Google‌ ‌CEO,‌ ‌Sundar‌ ‌Pichai,‌ ‌concisely‌ ‌illustrates‌ ‌the‌ ‌extent‌ ‌to‌ ‌
which‌ ‌artificial‌ ‌intelligence‌ ‌(AI)‌ ‌has‌ ‌impacted‌ ‌the‌ ‌world‌ ‌(Van‌ ‌de‌ ‌Gevel‌ ‌&‌ ‌Noussair,‌ ‌
2013).‌ ‌In‌ ‌short,‌ ‌AI‌ ‌is‌ ‌when‌ ‌“machines‌ ‌act‌ ‌intelligently”‌ ‌(New‌ ‌Scientist,‌ ‌2017),‌ ‌and‌ ‌yet,‌ ‌
there‌ ‌is‌ ‌no‌ ‌magic‌ ‌behind‌ ‌its‌ ‌underlying‌ ‌abilities;‌ ‌in‌ ‌fact,‌ ‌most‌ ‌of‌ ‌the‌ ‌traditional‌ ‌principles‌ ‌
behind‌ ‌AI‌ ‌are‌ ‌built‌ ‌from‌ ‌simple‌ ‌artificial‌ ‌neural‌ ‌networks‌ ‌(ANN)‌ ‌that‌ ‌represent‌ ‌known‌ ‌
biological‌ ‌structures‌ ‌in‌ ‌the‌ ‌brain,‌ ‌which‌ ‌are‌ ‌based‌ ‌on‌ ‌the‌ ‌accumulation‌ ‌of‌ ‌a‌ ‌number‌ ‌of‌ ‌
researchers’‌ ‌work.‌ ‌Some‌ ‌of‌ ‌the‌ ‌most‌ ‌notable‌ ‌theories‌ ‌are‌ ‌Aristotle’s‌ ‌philosophical‌ ‌idea‌ ‌
of‌ ‌associationism‌ ‌in‌ ‌300‌ ‌BC,‌ ‌and‌ ‌Donald‌ ‌Hebb’s‌ ‌Hebbian‌ ‌Learning‌ ‌Rule‌ ‌in‌ ‌1949.‌ ‌The‌ ‌
former‌ ‌states‌ ‌that‌ ‌the‌ ‌number‌ ‌of‌ ‌occurring‌ ‌events‌ ‌corresponds‌ ‌with‌ ‌the‌ ‌strength‌ ‌of‌ ‌their‌ ‌
connections;‌ ‌the‌ ‌‌latter‌ ‌expands‌ ‌upon‌ ‌that‌ ‌idea,‌ ‌explaining‌ ‌that‌,‌ ‌“cells‌ ‌that‌ ‌fire‌ ‌together,‌ ‌
wire‌ ‌together”‌ ‌(Wang‌ ‌&‌ ‌Raj,‌ ‌2017).‌ ‌Essentially,‌ ‌the‌ ‌strength‌ ‌of‌ ‌a‌ ‌connection‌ ‌is‌ ‌
proportional‌ ‌to‌ ‌its‌ ‌usage.‌ ‌
Thinkers‌ ‌have‌ ‌transformed‌ ‌these‌ ‌simple‌ ‌theories‌ ‌into‌ ‌the‌ ‌AI‌ ‌systems‌ ‌we‌ ‌are‌ ‌
familiar‌ ‌with‌ ‌today,‌ ‌such‌ ‌as‌ ‌Alexa’s‌ ‌natural-language‌ ‌predictions,‌ ‌Tesla’s‌ ‌self-driving‌ ‌
cars,‌ ‌and‌ ‌Netflix’s‌ ‌movie‌ ‌recommendations‌ ‌(Adams,‌ ‌2017).‌ ‌Yet,‌ ‌the‌ ‌non-biological‌ ‌
approach‌ ‌to‌ ‌artificial‌ ‌intelligence‌ ‌is‌ ‌not‌ ‌the‌ ‌only‌ ‌reason‌ ‌for‌ ‌its‌ ‌rapid‌ ‌progression;‌ ‌the‌ ‌field‌ ‌
of‌ ‌neuroscience‌ ‌has‌ ‌done‌ ‌just‌ ‌as‌ ‌well‌ ‌when‌ ‌implemented‌ ‌correctly.‌ ‌Unsurprisingly,‌ ‌since‌ ‌
4‌ ‌
the‌ ‌essence‌ ‌of‌ ‌AI‌ ‌is‌ ‌to‌ ‌model‌ ‌the‌ ‌learning‌ ‌capabilities‌ ‌of‌ ‌the‌ ‌brain‌ ‌and‌ ‌connect‌ ‌
computation‌ ‌to‌ ‌“intelligence”,‌ ‌many‌ ‌of‌ ‌the‌ ‌current‌ ‌algorithms,‌ ‌or‌ ‌computational‌ ‌functions‌ ‌
ran‌ ‌on‌ ‌computers,‌ ‌have‌ ‌been‌ ‌based‌ ‌on‌ ‌biological‌ ‌neurons,‌ ‌synapses,‌ ‌and‌ ‌neural‌ ‌
networks‌ ‌(Lomonaco‌ ‌&‌ ‌Maltoni,‌ ‌2015).‌ ‌It‌ ‌is‌ ‌popular‌ ‌to‌ ‌write‌ ‌algorithms‌ ‌that‌ ‌improve‌ ‌
upon‌ ‌these‌ ‌existing‌ ‌AI‌ ‌methods;‌ ‌however,‌ ‌there‌ ‌has‌ ‌been‌ ‌an‌ ‌effort‌ ‌to‌ ‌exercise‌ ‌more‌ ‌
neurological‌ ‌principles‌ ‌in‌ ‌order‌ ‌to‌ ‌model‌ ‌the‌ ‌human‌ ‌mind‌ ‌more‌ ‌accurately.‌ ‌While‌ ‌these‌ ‌
theories‌ ‌visit‌ ‌the‌ ‌hierarchical‌ ‌organization,‌ ‌cell‌ ‌specialization,‌ ‌neural‌ ‌activation,‌ ‌synaptic‌ ‌
sparsity,‌ ‌and‌ ‌plasticity‌ ‌of‌ ‌the‌ ‌brain‌ ‌(Hawkins,‌ ‌Lewis,‌ ‌Klukas,‌ ‌Purdy‌ ‌&‌ ‌Ahmad‌ ‌2019;‌ ‌
Ahmad‌ ‌&‌ ‌Scheinkman,‌ ‌2019;‌ ‌Miconi,‌ ‌Clune‌ ‌&‌ ‌Stanley,‌ ‌2018),‌ ‌there‌ ‌is‌ ‌a‌ ‌lack‌ ‌of‌ ‌holistic‌ ‌
concentration‌ ‌on‌ ‌any‌ ‌one,‌ ‌key‌ ‌feature.‌ ‌ ‌
 ‌
A‌ ‌Brief‌ ‌Overview‌ ‌of‌ ‌Neuroscience‌ ‌
Origins‌ ‌
From‌ ‌Hippocrates’‌ ‌antiquated‌ ‌theory‌ ‌that‌ ‌the‌ ‌brain‌ ‌is‌ ‌the‌ ‌seat‌ ‌of‌ ‌intelligence‌,‌ ‌to‌ ‌
Numenta’s‌ ‌Thousand‌ ‌Brains‌ ‌Theory‌ ‌of‌ ‌Intelligence‌ ‌‌—‌ ‌an‌ ‌effort‌ ‌to‌ ‌understand‌ ‌how‌ ‌the‌ ‌
brain‌ ‌computes‌ ‌numerous‌ ‌interpretations‌ ‌of‌ ‌observed‌ ‌objects‌ ‌(Numenta,‌ ‌2019)‌ ‌—‌ ‌
neuroscience‌ ‌has‌ ‌continued‌ ‌to‌ ‌lead‌ ‌researchers‌ ‌toward‌ ‌novel‌ ‌discoveries.‌ ‌To‌ ‌fully‌ ‌
understand‌ ‌the‌ ‌breadth‌ ‌of‌ ‌information‌ ‌we‌ ‌have‌ ‌today,‌ ‌it‌ ‌is‌ ‌imperative‌ ‌to‌ ‌highlight‌ ‌a‌ ‌few,‌ ‌
key‌ ‌developments‌ ‌in‌ ‌the‌ ‌field,‌ ‌before‌ ‌a‌ ‌modern‌ ‌interpretation‌ ‌of‌ ‌the‌ ‌brain’s‌ ‌functionality‌ ‌
can‌ ‌be‌ ‌understood‌ ‌as‌ ‌a‌ ‌whole.‌ ‌ ‌
In‌ ‌1825,‌ ‌Robert‌ ‌B.‌ ‌Todd‌ ‌discussed‌ ‌the‌ ‌role‌ ‌of‌ ‌the‌ ‌cerebral‌ ‌cortex‌ ‌in‌ ‌mental‌ ‌ ‌
5‌ ‌
activity‌ ‌(Chudler).‌ ‌As‌ ‌we‌ ‌understand‌ ‌it‌ ‌today,‌ ‌the‌ ‌majority‌ ‌of‌ ‌the‌ ‌cortex‌ ‌has‌ ‌been‌ ‌coined‌ ‌
the‌ ‌“neocortex”,‌ ‌which‌ ‌is‌ ‌a‌ ‌2-3‌ ‌millimeter‌ ‌thick‌ ‌covering‌ ‌of‌ ‌gray‌ ‌matter‌ ‌over‌ ‌the‌ ‌
cerebrum‌ ‌(Figure‌ ‌1),‌ ‌and‌ ‌contains‌ ‌six‌ ‌unique‌ ‌layers‌ ‌(Figure‌ ‌2)‌ ‌which‌ ‌govern‌ ‌the‌ ‌many‌ ‌
cortices‌ ‌—‌ ‌specific‌ ‌areas‌ ‌of‌ ‌function‌ ‌in‌ ‌the‌ ‌neocortex‌ ‌—‌ ‌that‌ ‌reside‌ ‌in‌ ‌each‌ ‌hemisphere‌ ‌
of‌ ‌the‌ ‌brain‌ ‌(Swenson,‌ ‌2006;‌ ‌Mayfield‌ ‌Clinic,‌ ‌2018).‌ ‌
 ‌ ‌
Fig.‌ ‌1.‌ ‌Drawing‌ ‌of‌ ‌cerebrum‌ ‌with‌ ‌four‌ ‌lobes‌ ‌on‌ ‌the‌ ‌left‌ ‌hemisphere‌ ‌of‌ ‌the‌ ‌brain.‌ ‌
6‌ ‌
 ‌
Fig.‌ ‌2.‌ ‌The‌ ‌six‌ ‌layers‌ ‌of‌ ‌the‌ ‌neocortex‌ ‌with‌ ‌various‌ ‌interconnected‌ ‌neurons‌ ‌(left),‌ ‌and‌ ‌a‌ ‌drawing‌ ‌of‌ ‌a‌ ‌neuron‌ ‌(right).‌ ‌
In‌ ‌each‌ ‌hemisphere,‌ ‌there‌ ‌are‌ ‌four‌ ‌main‌ ‌lobes:‌ ‌temporal,‌ ‌occipital,‌ ‌parietal,‌ ‌and‌ ‌ ‌
frontal.‌ ‌Respectively,‌ ‌they‌ ‌are‌ ‌responsible‌ ‌for‌ ‌organization‌ ‌and‌ ‌memory,‌ ‌visual‌ ‌
interpretation,‌ ‌sensory‌ ‌interpretation‌ ‌and‌ ‌spatial‌ ‌perception,‌ ‌and‌ ‌personality‌ ‌and‌ ‌
intelligence‌ ‌(Mayfield‌ ‌Clinic,‌ ‌2018);‌ ‌additionally,‌ ‌it‌ ‌is‌ ‌important‌ ‌to‌ ‌understand‌ ‌that‌ ‌each‌ ‌
have‌ ‌overlapping‌ ‌features‌ ‌that‌ ‌do‌ ‌not‌ ‌specialize‌ ‌in‌ ‌a‌ ‌single‌ ‌operation.‌ ‌From‌ ‌the‌ ‌various‌ ‌
parts‌ ‌of‌ ‌our‌ ‌brain,‌ ‌we‌ ‌are‌ ‌able‌ ‌to‌ ‌accomplish‌ ‌“intelligent”‌ ‌tasks‌ ‌(Swenson,‌ ‌2006).‌ ‌Rather‌ ‌
than‌ ‌in‌ ‌the‌ ‌cortices,‌ ‌the‌ ‌mystery‌ ‌behind‌ ‌these‌ ‌complex‌ ‌abilities‌ ‌lies‌ ‌within‌ ‌each‌ ‌layer‌ ‌of‌ ‌
the‌ ‌neocortex.‌ ‌In‌ ‌these‌ ‌layers,‌ ‌neurons‌ ‌form‌ ‌the‌ ‌basis‌ ‌for‌ ‌information‌ ‌processing,‌ ‌and‌ ‌
7‌ ‌
create‌ ‌large‌ ‌networks‌ ‌via‌ ‌their‌ ‌connective‌ ‌dendrites‌ ‌and‌ ‌axons.‌ ‌In‌ ‌1865,‌ ‌Otto‌ ‌Friedrich‌ ‌
Karl‌ ‌Deiters‌ ‌first‌ ‌differentiated‌ ‌between‌ ‌axons‌ ‌and‌ ‌dendrites‌ ‌(Chudler),‌ ‌but‌ ‌today‌ ‌we‌ ‌
know‌ ‌much‌ ‌more‌ ‌about‌ ‌the‌ ‌specific‌ ‌function‌ ‌of‌ ‌each‌ ‌structure.‌ ‌Neurons‌ ‌maintain‌ ‌a‌ ‌
resting‌ ‌potential‌ ‌of‌ ‌-70‌ ‌millivolts‌ ‌as‌ ‌ions‌ ‌such‌ ‌as‌ ‌sodium‌ ‌and‌ ‌potassium‌ ‌permeate‌ ‌the‌ ‌
cell‌ ‌membrane;‌ ‌ion‌ ‌channels‌ ‌keep‌ ‌the‌ ‌inside‌ ‌of‌ ‌the‌ ‌cell‌ ‌slightly‌ ‌more‌ ‌negative‌ ‌than‌ ‌the‌ ‌
outside.‌ ‌When‌ ‌some‌ ‌stimulus‌ ‌is‌ ‌received‌ ‌by‌ ‌the‌ ‌dendrites‌ ‌of‌ ‌a‌ ‌neuron,‌ ‌sodium‌ ‌channels‌ ‌
open,‌ ‌causing‌ ‌the‌ ‌neuron‌ ‌to‌ ‌become‌ ‌more‌ ‌positive‌ ‌—‌ ‌depolarize.‌ ‌If‌ ‌a‌ ‌certain‌ ‌threshold‌ ‌
of‌ ‌depolarization‌ ‌is‌ ‌reached,‌ ‌more‌ ‌sodium‌ ‌channels‌ ‌open,‌ ‌reaching‌ ‌an‌ ‌activation‌ ‌
potential‌ ‌which‌ ‌sends‌ ‌a‌ ‌signal‌ ‌that‌ ‌is‌ ‌propagated‌ ‌through‌ ‌the‌ ‌axon.‌ ‌When‌ ‌the‌ ‌signal‌ ‌
reaches‌ ‌the‌ ‌axon‌ ‌terminal,‌ ‌or‌ ‌the‌ ‌end‌ ‌of‌ ‌the‌ ‌axon,‌ ‌calcium‌ ‌ions‌ ‌release‌ ‌vesicles‌ ‌filled‌ ‌
with‌ ‌neurotransmitters‌ ‌across‌ ‌the‌ ‌synaptic‌ ‌cleft‌ ‌—‌ ‌the‌ ‌gap‌ ‌between‌ ‌the‌ ‌axon‌ ‌and‌ ‌
dendrite.‌ ‌These‌ ‌neurotransmitters‌ ‌are‌ ‌accepted‌ ‌by‌ ‌the‌ ‌receptors‌ ‌at‌ ‌the‌ ‌synapse‌ ‌of‌ ‌the‌ ‌
receiving‌ ‌neuron’s‌ ‌dendrite,‌ ‌which‌ ‌open‌ ‌more‌ ‌ion‌ ‌channels.‌ ‌This‌ ‌process‌ ‌repeats‌ ‌until‌ ‌a‌ ‌
neuron‌ ‌is‌ ‌unable‌ ‌to‌ ‌fire‌ ‌an‌ ‌activation‌ ‌potential‌ ‌(Chudler,‌ ‌2018;‌ ‌Kanin,‌ ‌Wro‌ń‌ska‌ ‌&‌ ‌‌Zięba,‌ ‌
2017;‌ ‌‌Stufflebeam,‌ ‌2008;‌ ‌Mayfield‌ ‌Clinic,‌ ‌2018;‌ ‌Chudler,‌ ‌2017).‌ ‌A‌ ‌slight‌ ‌nuance‌ ‌to‌ ‌the‌ ‌
exchange‌ ‌of‌ ‌neurotransmitters‌ ‌is‌ ‌that‌ ‌they‌ ‌may‌ ‌be‌ ‌stopped‌ ‌by‌ ‌diffusion‌ ‌(as‌ ‌
neurotransmitters‌ ‌drift‌ ‌away),‌ ‌enzymatic‌ ‌degradation‌ ‌(when‌ ‌enzymes‌ ‌break‌ ‌down‌ ‌
neurotransmitters,‌ ‌rendering‌ ‌them‌ ‌unrecognizable‌ ‌to‌ ‌receptors),‌ ‌removal‌ ‌by‌ ‌glial‌ ‌cells,‌ ‌
or‌ ‌reuptake‌ ‌(where‌ ‌neurotransmitters‌ ‌are‌ ‌taken‌ ‌back‌ ‌into‌ ‌the‌ ‌axon‌ ‌terminal)‌ ‌(Chudler,‌ ‌
2017).‌ ‌This‌ ‌is‌ ‌done‌ ‌to‌ ‌remove‌ ‌excess‌ ‌neurotransmitters,‌ ‌so‌ ‌that‌ ‌they‌ ‌do‌ ‌not‌ ‌continue‌ ‌to‌ ‌
incite‌ ‌activation‌ ‌of‌ ‌a‌ ‌neuron‌ ‌(Williams‌ ‌College‌ ‌Neuroscience,‌ ‌1998;‌  ‌Frye,‌ ‌2016).‌ ‌This‌ ‌
8‌ ‌
process‌ ‌of‌ ‌neural‌ ‌connectivity‌ ‌can‌ ‌be‌ ‌followed‌ ‌in‌ ‌Figure‌ ‌3,‌ ‌as‌ ‌a‌ ‌message‌ ‌is‌ ‌passed‌ ‌from‌ ‌
the‌ ‌dendrites‌ ‌to‌ ‌the‌ ‌synapse.‌ ‌
 ‌
Fig.‌ ‌3.‌ ‌A‌ ‌neuron‌ ‌transmitting‌ ‌a‌ ‌signal‌ ‌to‌ ‌another‌ ‌neuron‌ ‌at‌ ‌the‌ ‌synapse.‌ ‌
 ‌
These‌ ‌connections‌ ‌work‌ ‌in‌ ‌a‌ ‌system‌ ‌of‌ ‌layers‌ ‌within‌ ‌the‌ ‌neocortex‌ ‌to‌ ‌relay‌ ‌information‌ ‌
to‌ ‌specific‌ ‌cortices‌ ‌for‌ ‌various‌ ‌brain‌ ‌functions.‌ ‌Knowing‌ ‌the‌ ‌hierarchy‌ ‌of‌ ‌the‌ ‌neocortex‌ ‌
—‌ ‌two‌ ‌hemispheres‌ ‌divided‌ ‌into‌ ‌four‌ ‌lobes‌ ‌each,‌ ‌with‌ ‌multiple‌ ‌specialized‌ ‌cortices‌ ‌
throughout,‌ ‌and‌ ‌six‌ ‌layers‌ ‌deep‌ ‌with‌ ‌densely-linked‌ ‌neurons‌ ‌—‌ ‌it‌ ‌is‌ ‌possible‌ ‌to‌ ‌
understand‌ ‌how‌ ‌the‌ ‌brain‌ ‌utilizes‌ ‌connectivity,‌ ‌which‌ ‌is‌ ‌integral‌ ‌to‌ ‌how‌ ‌it‌ ‌changes‌ ‌and‌ ‌
optimizes‌ ‌itself‌ ‌over‌ ‌time.‌ ‌
 ‌
Plasticity‌ ‌
9‌ ‌
Two-thirds‌ ‌of‌ ‌the‌ ‌10-16‌ ‌billion‌ ‌neurons‌ ‌in‌ ‌the‌ ‌neocortex‌ ‌are‌ ‌pyramidal,‌ ‌each‌ ‌of‌ ‌
which‌ ‌receive‌ ‌thousands‌ ‌of‌ ‌synaptic‌ ‌inputs‌ ‌(Swenson,‌ ‌2006;‌ ‌Mayfield‌ ‌Clinic,‌ ‌2018;‌ ‌
Hawkins‌ ‌&‌ ‌Ahmad,‌ ‌2016;‌ ‌Masland,‌ ‌2004).‌ ‌In‌ ‌the‌ ‌pyramidal‌ ‌neuron,‌ ‌as‌ ‌well‌ ‌as‌ ‌most‌ ‌
other‌ ‌neuronal‌ ‌cells,‌ ‌the‌ ‌strength‌ ‌and‌ ‌arrangement‌ ‌of‌ ‌connections‌ ‌changes‌ ‌at‌ ‌the‌ ‌
synapse;‌ ‌this‌ ‌is‌ ‌called‌ ‌“plasticity”.‌ ‌Plasticity‌ ‌is‌ ‌the‌ ‌process‌ ‌in‌ ‌which‌ ‌our‌ ‌brain‌ ‌learns‌ ‌and‌ ‌
adapts‌ ‌to‌ ‌a‌ ‌constantly‌ ‌changing‌ ‌perception‌ ‌of‌ ‌the‌ ‌world,‌ ‌and‌ ‌underlies‌ ‌the‌ ‌core‌ ‌
functionality‌ ‌of‌ ‌the‌ ‌human‌ ‌brain‌ ‌as‌ ‌a‌ ‌whole‌ ‌‌(Kanin,‌ ‌Wro‌ń‌ska‌ ‌&‌ ‌‌Zięba,‌ ‌2017).‌ ‌
Two‌ ‌of‌ ‌the‌ ‌most‌ ‌important‌ ‌features‌ ‌of‌ ‌plasticity‌ ‌are‌ ‌long‌ ‌term‌ ‌potentiation‌ ‌and‌ ‌ ‌
long‌ ‌term‌ ‌depression,‌ ‌also‌ ‌known‌ ‌as‌ ‌LTP‌ ‌and‌ ‌LTD.‌ ‌Respectively,‌ ‌each‌ ‌process‌ ‌
strengthens‌ ‌and‌ ‌weakens‌ ‌synaptic‌ ‌strength.‌ ‌This‌ ‌change‌ ‌is‌ ‌due‌ ‌to‌ ‌synaptic‌ ‌history:‌ ‌the‌ ‌
number‌ ‌of‌ ‌times‌ ‌a‌ ‌synapse‌ ‌has‌ ‌been‌ ‌used‌ ‌is‌ ‌directly‌ ‌related‌ ‌to‌ ‌its‌ ‌strength‌ ‌‌(Kanin,‌ ‌
Wro‌ń‌ska‌ ‌&‌ ‌‌Zięba,‌ ‌2017);‌ ‌neurons‌ ‌will‌ ‌either‌ ‌pull‌ ‌in‌ ‌or‌ ‌put‌ ‌out‌ ‌more‌ ‌receptors,‌ ‌based‌ ‌on‌ ‌
the‌ ‌amount‌ ‌of‌ ‌synaptic‌ ‌input‌ ‌received‌ ‌(Trafton,‌ ‌2016).‌ ‌This‌ ‌means‌ ‌that‌ ‌the‌ ‌neurons‌ ‌that‌ ‌
are‌ ‌very‌ ‌active‌ ‌will‌ ‌have‌ ‌synapses‌ ‌with‌ ‌more‌ ‌receptors‌ ‌than‌ ‌those‌ ‌that‌ ‌are‌ ‌inactive;‌ ‌
therefore‌ ‌more‌ ‌neurotransmitters‌ ‌will‌ ‌be‌ ‌connected‌ ‌with‌ ‌receptors,‌ ‌opening‌ ‌more‌ ‌ion‌ ‌
channels.‌ ‌Effectively,‌ ‌LTP‌ ‌and‌ ‌LTD‌ ‌control‌ ‌the‌ ‌activation‌ ‌potential‌ ‌in‌ ‌the‌ ‌neuron‌ ‌
(Thomson,‌ ‌2000).‌ ‌
Another‌ ‌necessary‌ ‌function‌ ‌in‌ ‌the‌ ‌brain‌ ‌is‌ ‌homeostatic‌ ‌plasticity.‌ ‌This‌ ‌is‌ ‌because‌ ‌
“when‌ ‌synapses‌ ‌undergo‌ ‌LTP‌ ‌they‌ ‌are‌ ‌better‌ ‌able‌ ‌to‌ ‌depolarize‌ ‌the‌ ‌postsynaptic‌ ‌
neurons,‌ ‌which‌ ‌will‌ ‌increase‌ ‌the‌ ‌probability‌ ‌that‌ ‌they‌ ‌will‌ ‌undergo‌ ‌further‌ ‌LTP‌ ‌—‌ ‌leading‌ ‌
to‌ ‌unconstrained‌ ‌synaptic‌ ‌strengthening”‌ ‌(Turrigiano,‌ ‌2012).‌ ‌In‌ ‌order‌ ‌to‌ ‌combat‌ ‌this‌ ‌
snowball‌ ‌effect‌ ‌of‌ ‌synaptic‌ ‌strengthening,‌ ‌homeostatic‌ ‌plasticity‌ ‌regulates‌ ‌the‌ ‌threshold‌ ‌
10‌ ‌
for‌ ‌synaptic‌ ‌firing‌ ‌‌(Kanin,‌ ‌Wro‌ń‌ska‌ ‌&‌ ‌‌Zięba,‌ ‌2017).‌ ‌One‌ ‌method‌ ‌in‌ ‌which‌ ‌firing‌ ‌is‌ ‌
restrained‌ ‌is‌ ‌via‌ ‌synaptic‌ ‌scaling,‌ ‌where‌ ‌synaptic‌ ‌strength‌ ‌is‌ ‌scaled‌ ‌down‌ ‌in‌ ‌accordance‌ ‌
to‌ ‌its‌ ‌activity‌ ‌—‌ ‌synaptic‌ ‌scaling‌ ‌can‌ ‌be‌ ‌seen‌ ‌in‌ ‌action‌ ‌in‌ ‌Figure‌ ‌N.;‌ ‌this‌ ‌function‌ ‌will‌ ‌be‌ ‌
my‌ ‌central‌ ‌focus‌ ‌when‌ ‌addressing‌ ‌homeostatic‌ ‌functionality‌ ‌in‌ ‌my‌ ‌methodology‌ ‌section‌ ‌
(Turrigiano,‌ ‌2012).‌ ‌The‌ ‌homeostatic‌ ‌effect‌ ‌can‌ ‌also‌ ‌be‌ ‌seen‌ ‌in‌ ‌a‌ ‌study‌ ‌from‌ ‌the‌ ‌
Massachusetts‌ ‌Institute‌ ‌of‌ ‌Technology,‌ ‌where‌ ‌mice‌ ‌were‌ ‌shown‌ ‌targets‌ ‌in‌ ‌different‌ ‌
receptive‌ ‌fields‌ ‌and‌ ‌flashed‌ ‌with‌ ‌blue‌ ‌light‌ ‌when‌ ‌the‌ ‌target‌ ‌was‌ ‌moved.‌ ‌This‌ ‌optical‌ ‌
stimulation‌ ‌caused‌ ‌particular‌ ‌synapses‌ ‌to‌ ‌strengthen.‌ ‌When‌ ‌looked‌ ‌at‌ ‌through‌ ‌a‌ ‌
two-photon‌ ‌microscope,‌ ‌neighboring‌ ‌synapses‌ ‌to‌ ‌the‌ ‌strengthened‌ ‌synapse‌ ‌had‌ ‌shrank‌ ‌
(Orenstein,‌ ‌2018),‌ ‌effectively‌ ‌scaling‌ ‌each‌ ‌local‌ ‌synapse.‌ ‌
 ‌
Fig.‌ ‌N.‌ ‌Synaptic‌ ‌scaling‌ ‌via‌ ‌homeostatic‌ ‌plasticity.‌ ‌
 ‌
Ultimately,‌ ‌the‌ ‌relationship‌ ‌between‌ ‌the‌ ‌activation‌ ‌potential,‌ ‌LTP‌ ‌LTD,‌ ‌and‌ ‌
homeostatic‌ ‌plasticity‌ ‌are‌ ‌what‌ ‌define‌ ‌the‌ ‌essence‌ ‌of‌ ‌plasticity.‌ ‌However‌ ‌narrow‌ ‌this‌ ‌
biological‌ ‌function‌ ‌is,‌ ‌plasticity‌ ‌is‌ ‌a‌ ‌major‌ ‌contributor‌ ‌to‌ ‌intelligence,‌ ‌and‌ ‌must‌ ‌be‌ ‌
11‌ ‌
understood‌ ‌in‌ ‌conjunction‌ ‌with‌ ‌neural‌ ‌connectivity‌ ‌in‌ ‌order‌ ‌to‌ ‌create‌ ‌true‌ ‌artificial‌ ‌
intelligence.‌ ‌
 ‌
A‌ ‌Brief‌ ‌Overview‌ ‌of‌ ‌Artificial‌ ‌Intelligence‌ ‌
Origins‌ ‌
The‌ ‌term‌ ‌“artificial‌ ‌intelligence”‌ ‌was‌ ‌not‌ ‌coined‌ ‌until‌ ‌1956‌ ‌by‌ ‌a‌ ‌small‌ ‌gathering‌ ‌of‌ ‌
research‌ ‌scientists‌ ‌at‌ ‌Dartmouth‌ ‌(Dartmouth‌ ‌College,‌ ‌2019),‌ ‌and‌ ‌yet,‌ ‌major‌ ‌
breakthroughs‌ ‌in‌ ‌the‌ ‌emerging‌ ‌field‌ ‌were‌ ‌made‌ ‌incredibly‌ ‌quickly.‌ ‌Similar‌ ‌to‌ ‌the‌ ‌
overview‌ ‌of‌ ‌neuroscience,‌ ‌the‌ ‌elucidation‌ ‌of‌ ‌major‌ ‌events‌ ‌in‌ ‌the‌ ‌field‌ ‌of‌ ‌AI‌ ‌will‌ ‌help‌ ‌
provide‌ ‌a‌ ‌proper‌ ‌understanding‌ ‌of‌ ‌modern‌ ‌theory.‌ ‌
Before‌ ‌Donald‌ ‌Hebb’s‌ ‌Hebbian‌ ‌Learning‌ ‌Rule,‌ ‌the‌ ‌MCP‌ ‌neural‌ ‌model‌ ‌was‌ ‌ ‌
conceived‌ ‌in‌ ‌1943.‌ ‌Designed‌ ‌by‌ ‌Warren‌ ‌McCulloch‌ ‌and‌ ‌Walter‌ ‌Pitts‌ ‌(hence‌ ‌MCP),‌ ‌the‌ ‌
model‌ ‌utilized‌ ‌various‌ ‌key‌ ‌neurological‌ ‌principles‌ ‌such‌ ‌as‌ ‌the‌ ‌usage‌ ‌of‌ ‌weights‌ ‌‌—‌‌ ‌to‌ ‌
represent‌ ‌synapses‌ ‌connected‌ ‌to‌ ‌neurons‌ ‌‌—‌ ‌‌and‌ ‌threshold‌ ‌activation‌ ‌‌—‌ ‌‌to‌ ‌simulate‌ ‌the‌ ‌
neurological‌ ‌action‌ ‌potential.‌ ‌However,‌ ‌the‌ ‌“perceptron”,‌ ‌designed‌ ‌by‌ ‌Frank‌ ‌Rosenblatt‌ ‌
in‌ ‌1958,‌ ‌formed‌ ‌the‌ ‌basis‌ ‌of‌ ‌the‌ ‌popularly‌ ‌utilized‌ ‌“neural‌ ‌networks”‌ ‌that‌ ‌we‌ ‌see‌ ‌today.‌ ‌
As‌ ‌seen‌ ‌in‌ ‌Figure‌ ‌4,‌ ‌the‌ ‌design‌ ‌resembles‌ ‌a‌ ‌neuron‌ ‌with‌ ‌multiple‌ ‌synapses,‌ ‌where‌ ‌input‌ ‌
is‌ ‌carried‌ ‌through‌ ‌the‌ ‌weights‌ ‌and‌ ‌summed‌ ‌at‌ ‌the‌ ‌neuron,‌ ‌yet,‌ ‌the‌ ‌idea‌ ‌of‌ ‌a‌ ‌threshold‌ ‌is‌ ‌
abandoned‌ ‌(Wang‌ ‌&‌ ‌Raj,‌ ‌2017;‌ ‌LeCun,‌ ‌Bengio‌ ‌&‌ ‌Hinton,‌ ‌2015).‌ ‌Even‌ ‌without‌ ‌heavy‌ ‌
neurological‌ ‌influence,‌ ‌the‌ ‌first‌ ‌perceptron‌ ‌is‌ ‌widely‌ ‌acknowledged‌ ‌for‌ ‌its‌ ‌role‌ ‌in‌ ‌the‌ ‌
creation‌ ‌of‌ ‌artificial‌ ‌intelligence.‌ ‌
12‌ ‌
 ‌
Fig.‌ ‌4.‌ ‌A‌ ‌classical‌ ‌perceptron.‌ ‌
It‌ ‌is‌ ‌understood‌ ‌that‌ ‌the‌ ‌work‌ ‌of‌ ‌McCulloch,‌ ‌Pitts,‌ ‌and‌ ‌Rosenblatt‌ ‌contributed‌ ‌to‌ ‌a‌ ‌ ‌
solid‌ ‌representation‌ ‌of‌ ‌how‌ ‌information‌ ‌propagates‌ ‌forward‌ ‌in‌ ‌the‌ ‌brain‌ ‌by‌ ‌using‌ ‌models‌ ‌
similar‌ ‌to‌ ‌Figure‌ ‌4,‌ ‌and‌ ‌yet,‌ ‌a‌ ‌proper‌ ‌method‌ ‌of‌ ‌self-learning‌ ‌was‌ ‌not‌ ‌published‌ ‌until‌ ‌
1986.‌ ‌In‌ ‌a‌ ‌paper‌ ‌by‌ ‌David‌ ‌Rumelhart,‌ ‌Geoffrey‌ ‌Hinton,‌ ‌and‌ ‌Ronald‌ ‌Williams,‌ ‌the‌ ‌
method‌ ‌of‌ ‌“backpropagation”‌ ‌was‌ ‌used‌ ‌to‌ ‌alter‌ ‌weights‌ ‌in‌ ‌order‌ ‌to‌ ‌optimize‌ ‌a‌ ‌neural‌ ‌
network‌ ‌as‌ ‌a‌ ‌whole‌ ‌(Rumelhart,‌ ‌Hinton‌ ‌&‌ ‌Williams,‌ ‌1986;‌ ‌McGonagle,‌ ‌Shaikouski,‌ ‌
Williams,‌ ‌Hsu‌ ‌&‌ ‌Khim,‌ ‌2019).‌ ‌Optimization‌ ‌in‌ ‌this‌ ‌context‌ ‌refers‌ ‌to‌ ‌a‌ ‌system‌ ‌getting‌ ‌
increasingly‌ ‌better‌ ‌at‌ ‌performing‌ ‌“intelligent”‌ ‌tasks,‌ ‌such‌ ‌as‌ ‌answering‌ ‌questions‌ ‌after‌ ‌
reading‌ ‌a‌ ‌story,‌ ‌or‌ ‌describing‌ ‌objects‌ ‌in‌ ‌a‌ ‌picture‌ ‌(LeCun,‌ ‌Bengio‌ ‌&‌ ‌Hinton,‌ ‌2015).‌ ‌
Today,‌ ‌backpropagation‌ ‌is‌ ‌used‌ ‌as‌ ‌a‌ ‌first-choice‌ ‌optimization‌ ‌method.‌ ‌
Together,‌ ‌forward‌ ‌propagation‌ ‌and‌ ‌backpropagation‌ ‌have‌ ‌effectively‌ ‌built‌ ‌upon‌ ‌
previously‌ ‌established‌ ‌theories‌ ‌of‌ ‌intelligence‌ ‌in‌ ‌order‌ ‌to‌ ‌both‌ ‌simulate‌ ‌the‌ ‌brain,‌ ‌and‌ ‌
provide‌ ‌optimal‌ ‌predictions.‌ ‌ ‌
13‌ ‌
Existing‌ ‌Optimization‌ ‌Success‌ ‌
Although‌ ‌great‌ ‌in‌ ‌theory,‌ ‌there‌ ‌is‌ ‌a‌ ‌reason‌ ‌why‌ ‌neuroscience‌ ‌hasn’t‌ ‌always‌ ‌been‌ ‌ ‌
the‌ ‌focal‌ ‌point‌ ‌of‌ ‌artificial‌ ‌intelligence.‌ ‌In‌ ‌fact,‌ ‌the‌ ‌most‌ ‌successful‌ ‌AI‌ ‌has‌ ‌already‌ ‌begun‌ ‌
to‌ ‌outperform‌ ‌humans‌ ‌in‌ ‌intelligent‌ ‌tasks.‌ ‌For‌ ‌example,‌ ‌AlphaStar,‌ ‌an‌ ‌artificially‌ ‌
intelligent‌ ‌“Starcraft‌ ‌II”‌ ‌player‌ ‌‌—‌ ‌ ‌“a‌ ‌real-time‌ ‌strategy‌ ‌game‌ ‌in‌ ‌which‌ ‌players‌ ‌balance‌ ‌
high-level‌ ‌economic‌ ‌decisions‌ ‌with‌ ‌individual‌ ‌control‌ ‌of‌ ‌hundreds‌ ‌of‌ ‌units”‌ ‌‌—‌ ‌ ‌was‌ ‌able‌ ‌
to‌ ‌achieve‌ ‌a‌ ‌ranking‌ ‌above‌ ‌99.8%‌ ‌of‌ ‌officially‌ ‌ranked‌ ‌human‌ ‌players‌ ‌(Vinyals‌ ‌et‌ ‌al.,‌ ‌
2019).‌ ‌The‌ ‌artificially‌ ‌intelligent,‌ ‌AlphaZero,‌ ‌was‌ ‌able‌ ‌to‌ ‌master‌ ‌chess,‌ ‌shogi‌ ‌(Japanese‌ ‌
chess),‌ ‌and‌ ‌Go,‌ ‌using‌ ‌nuanced‌ ‌neural‌ ‌networks‌ ‌not‌ ‌so‌ ‌dissimilar‌ ‌to‌ ‌AlphaStar’s‌ ‌(Silver‌ ‌
et‌ ‌al.,‌ ‌2017).‌ ‌There‌ ‌is‌ ‌even‌ ‌an‌ ‌algorithm,‌ ‌GauGAN,‌ ‌that‌ ‌allows‌ ‌users‌ ‌to‌ ‌digitally‌ ‌paint‌ ‌a‌ ‌
picture‌ ‌using‌ ‌colors‌ ‌that‌ ‌represent‌ ‌water,‌ ‌gravel,‌ ‌clouds,‌ ‌etc.‌ ‌(Figure‌ ‌5),‌ ‌and‌ ‌watch‌ ‌it‌ ‌
transform‌ ‌into‌ ‌photorealistic‌ ‌recreation‌ ‌(Figure‌ ‌6).‌ ‌This‌ ‌type‌ ‌of‌ ‌neural‌ ‌network‌ ‌is‌ ‌called‌ ‌a‌ ‌
Generative‌ ‌Adversarial‌ ‌Network‌ ‌(GAN)‌ ‌(Park,‌ ‌Liu,‌ ‌Wang‌ ‌&‌ ‌Zhu,‌ ‌2019).‌ ‌ ‌
 ‌
14‌ ‌
Fig.‌ ‌5.‌ ‌&‌ ‌Fig.‌ ‌6.‌ ‌A‌ ‌picture‌ ‌that‌ ‌I‌ ‌drew‌ ‌using‌ ‌the‌ ‌GauGAN‌ ‌interactive‌ ‌demo‌ ‌(left),‌ ‌as‌ ‌input‌ ‌for‌ ‌the‌ ‌algorithm‌ ‌to‌ ‌create‌ ‌a‌ ‌
semi-photorealistic‌ ‌image‌ ‌(right).‌ ‌ ‌
 ‌
Aside‌ ‌from‌ ‌recreational‌ ‌advances,‌ ‌AI‌ ‌has‌ ‌been‌ ‌invaluable‌ ‌to‌ ‌the‌ ‌medical‌ ‌field‌ ‌ ‌
too.‌ ‌After‌ ‌being‌ ‌trained‌ ‌with‌ ‌68,000‌ ‌annotated‌ ‌liver‌ ‌biopsy‌ ‌images,‌ ‌PathAI’s‌ ‌algorithm‌ ‌
had‌ ‌very‌ ‌similar‌ ‌interpretations‌ ‌to‌ ‌75‌ ‌board‌ ‌certified‌ ‌pathologists,‌ ‌and‌ ‌were‌ ‌able‌ ‌to‌ ‌
make‌ ‌accurate‌ ‌predictions‌ ‌on‌ ‌developments‌ ‌such‌ ‌as‌ ‌the‌ ‌staging‌ ‌of‌ ‌fibrosis‌ ‌(Wilkinson,‌ ‌
2019).‌ ‌Again,‌ ‌this‌ ‌was‌ ‌all‌ ‌done‌ ‌using‌ ‌current‌ ‌techniques‌ ‌of‌ ‌machine‌ ‌intelligence,‌ ‌albeit‌ ‌
more‌ ‌intricate‌ ‌than‌ ‌a‌ ‌simple‌ ‌neural‌ ‌network,‌ ‌but‌ ‌built‌ ‌using‌ ‌the‌ ‌same‌ ‌principles.‌ ‌ ‌
Researchers‌ ‌have‌ ‌nonetheless‌ ‌begun‌ ‌to‌ ‌reach‌ ‌a‌ ‌plateau‌ ‌in‌ ‌the‌ ‌advancement‌ ‌of‌ ‌
artificial‌ ‌intelligence,‌ ‌because‌ ‌while‌ ‌algorithms‌ ‌are‌ ‌able‌ ‌to‌ ‌master‌ ‌complex‌ ‌games,‌ ‌they‌ ‌
are‌ ‌still‌ ‌unable‌ ‌to‌ ‌think‌ ‌creatively,‌ ‌empathize‌ ‌with,‌ ‌or‌ ‌otherwise‌ ‌act‌ ‌human.‌ ‌Artificial‌ ‌
intelligence‌ ‌in‌ ‌its‌ ‌current‌ ‌state‌ ‌is‌ ‌more‌ ‌about‌ ‌optimization‌ ‌than‌ ‌intelligence;‌ ‌there‌ ‌has‌ ‌
never‌ ‌been‌ ‌a‌ ‌better‌ ‌time‌ ‌to‌ ‌examine‌ ‌neuroscience‌ ‌more‌ ‌closely.‌ ‌
 ‌
Existing‌ ‌Neural‌ ‌Connectivity‌ ‌and‌ ‌Artificial‌ ‌Plasticity‌ ‌
Some‌ ‌of‌ ‌the‌ ‌leading‌ ‌theories‌ ‌in‌ ‌both‌ ‌theoretical‌ ‌neuroscience‌ ‌and‌ ‌AI‌ ‌research‌ ‌ ‌
are‌ ‌from‌ ‌Numenta:‌ ‌The‌ ‌Thousand‌ ‌Brains‌ ‌Theory‌ ‌of‌ ‌Intelligence‌ ‌(TTBTI)‌ ‌and‌ ‌
Hierarchical‌ ‌Temporal‌ ‌Memory‌ ‌(HTM)‌ ‌theory.‌ ‌In‌ ‌these‌ ‌two‌ ‌theories,‌ ‌the‌ ‌multilayered‌ ‌
cortical‌ ‌columns‌ ‌in‌ ‌the‌ ‌neocortex‌ ‌are‌ ‌responsible‌ ‌for‌ ‌the‌ ‌intelligence‌ ‌in‌ ‌the‌ ‌brain.‌ ‌The‌ ‌
latter‌ ‌theory‌ ‌is‌ ‌expanded‌ ‌upon‌ ‌by‌ ‌the‌ ‌former,‌ ‌because‌ ‌it‌ ‌states‌ ‌that‌ ‌the‌ ‌hierarchy‌ ‌within‌ ‌
cortical‌ ‌columns‌ ‌determines‌ ‌various,‌ ‌novel‌ ‌representations‌ ‌of‌ ‌the‌ ‌perceived‌ ‌world‌ ‌which‌ ‌
then‌ ‌consolidate‌ ‌on‌ ‌an‌ ‌answer‌ ‌or‌ ‌prediction‌ ‌(Numenta,‌ ‌2019;‌ ‌Hawkins,‌ ‌Lewis,‌ ‌Klukas,‌ ‌
15‌ ‌
Purdy‌ ‌&‌ ‌Ahmad,‌ ‌2019).‌ ‌Additionally,‌ ‌sparsity‌ ‌amongst‌ ‌neurons,‌ ‌or‌ ‌a‌ ‌limit‌ ‌on‌ ‌the‌ ‌number‌ ‌
of‌ ‌active‌ ‌neurons,‌ ‌is‌ ‌important‌ ‌for‌ ‌the‌ ‌robustness‌ ‌of‌ ‌neural‌ ‌systems‌ ‌to‌ ‌closely-related‌ ‌
input‌ ‌data‌ ‌(Numenta,‌ ‌2019;‌ ‌Ahmad‌ ‌&‌ ‌Sheinkman,‌ ‌2019).‌ ‌For‌ ‌the‌ ‌purposes‌ ‌of‌ ‌my‌ ‌
research‌ ‌I‌ ‌will‌ ‌be‌ ‌focusing‌ ‌solely‌ ‌on‌ ‌the‌ ‌HTM‌ ‌model,‌ ‌since‌ ‌it‌ ‌utilizes‌ ‌the‌ ‌principles‌ ‌of‌ ‌
neural‌ ‌connectivity‌ ‌and‌ ‌plasticity‌ ‌that‌ ‌have‌ ‌influenced‌ ‌the‌ ‌biological‌ ‌equations‌ ‌expanded‌ ‌
upon‌ ‌in‌ ‌the‌ ‌methodology‌ ‌section.‌ ‌In‌ ‌practice,‌ ‌HTM‌ ‌models‌ ‌tend‌ ‌to‌ ‌utilize‌ ‌principles‌ ‌of‌ ‌
Hebbian‌ ‌plasticity‌ ‌(since‌ ‌"HTM‌ ‌synaptic‌ ‌plasticity‌ ‌rule‌ ‌is‌ ‌a‌ ‌Hebbian-like‌ ‌rule")‌ ‌without‌ ‌it‌ ‌
being‌ ‌a‌ ‌central‌ ‌focus.‌ ‌These‌ ‌models‌ ‌use‌ ‌a‌ ‌combination‌ ‌of‌ ‌neural‌ ‌sparsity‌ ‌(i.e.‌ ‌low‌ ‌
percentage‌ ‌of‌ ‌active‌ ‌neurons),‌ ‌and‌ ‌NMDA‌ ‌spiking‌ ‌(i.e.‌ ‌the‌ ‌depolarization‌ ‌of‌ ‌a‌ ‌neuron‌ ‌
causes‌ ‌an‌ ‌activation‌ ‌potential;‌ ‌this‌ ‌approach‌ ‌can‌ ‌be‌ ‌seen‌ ‌in‌ ‌Figure‌ ‌7).‌ ‌Additionally,‌ ‌the‌ ‌
HTM‌ ‌network‌ ‌utilizes‌ ‌functions‌ ‌of‌ ‌LTP‌ ‌and‌ ‌LTD,‌ ‌both‌ ‌of‌ ‌which‌ ‌are‌ ‌integral‌ ‌to‌ ‌plasticity.‌ ‌
Figure‌ ‌8‌ ‌is‌ ‌Numenta’s‌ ‌mathematical‌ ‌approach‌ ‌to‌ ‌this‌ ‌phenomena,‌ ‌and‌ ‌is‌ ‌one‌ ‌of‌ ‌six‌ ‌
major‌ ‌equations‌ ‌that‌ ‌defines‌ ‌the‌ ‌learning‌ ‌and‌ ‌activation‌ ‌rules‌ ‌for‌ ‌their‌ ‌model‌ ‌(Hawkins‌ ‌&‌ ‌
Ahmad,‌ ‌2016),‌ ‌not‌ ‌all‌ ‌equations‌ ‌are‌ ‌included‌ ‌for‌ ‌the‌ ‌sake‌ ‌of‌ ‌simplicity.‌ ‌
 ‌
Fig.‌ ‌7.‌ ‌This‌ ‌equation‌ ‌demonstrates‌ ‌how,‌ ‌if‌ ‌the‌ ‌number‌ ‌of‌ ‌all‌ ‌active‌ ‌dendrites‌ ‌(‌Dij~d∘At)‌ ‌connected‌ ‌to‌ ‌a‌ ‌neuron‌ ‌exceeds‌ ‌a‌ ‌spiking‌ ‌
threshold‌ ‌(‌θ),‌ ‌an‌ ‌activation‌ ‌potential‌ ‌will‌ ‌(‌1)‌ ‌occur;‌ ‌otherwise‌ ‌it‌ ‌will‌ ‌not‌ ‌(‌0).‌ ‌
 ‌
Fig.‌ ‌8.‌ ‌This‌ ‌equation‌ ‌demonstrates‌ ‌how‌ ‌previously‌ ‌activated‌ ‌(‌At−1)‌ ‌dendrites‌ ‌(‌Dij·d)‌ ‌are‌ ‌strengthened‌ ‌(‌p+)‌ ‌while‌ ‌all‌ ‌dendrites‌ ‌are‌ ‌
uniformly‌ ‌weakened‌ ‌by‌ ‌a‌ ‌smaller‌ ‌value‌ ‌(p−),‌ ‌to‌ ‌distinguish‌ ‌long‌ ‌term‌ ‌potentiation‌ ‌from‌ ‌depression.‌ ‌
 ‌
16‌ ‌
In‌ ‌theory,‌ ‌HTM‌ ‌should‌ ‌work‌ ‌because‌ ‌of‌ ‌its‌ ‌neurological‌ ‌roots,‌ ‌and‌ ‌therefore‌ ‌it‌ ‌
should‌ ‌not‌ ‌be‌ ‌too‌ ‌surprising‌ ‌that‌ ‌it‌ ‌does.‌ ‌When‌ ‌compared‌ ‌to‌ ‌three‌ ‌other‌ ‌neural‌ ‌models‌ ‌
—‌ ‌“nearest‌ ‌neighbor‌ ‌(NN)”,‌ ‌“multilayer‌ ‌perceptron‌ ‌(MLP)”,‌ ‌“convolutional‌ ‌network‌ ‌
(LeNet)”‌ ‌—‌ ‌on‌ ‌the‌ ‌SDIGIT‌ ‌data‌ ‌set‌ ‌of‌ ‌numbers,‌ ‌it‌ ‌did‌ ‌better‌ ‌by‌ ‌a‌ ‌margin‌ ‌of‌ ‌4.09%‌ ‌
(71.37%‌ ‌accuracy),‌ ‌8.25%‌ ‌(87.56%‌ ‌accuracy),‌ ‌and‌ ‌5.44%‌ ‌(94.61%‌ ‌accuracy).‌ ‌Each‌ ‌
test‌ ‌was‌ ‌done‌ ‌with‌ ‌an‌ ‌increasing‌ ‌number‌ ‌of‌ ‌training‌ ‌data‌ ‌‌(Rehn‌ ‌&‌ ‌Maltoni,‌ ‌2014).‌ ‌
Another‌ ‌example‌ ‌is‌ ‌the‌ ‌success‌ ‌of‌ ‌an‌ ‌implemented‌ ‌HTM‌ ‌model‌ ‌on‌ ‌the‌ ‌NORB‌ ‌dataset;‌ ‌
the‌ ‌network‌ ‌would‌ ‌have‌ ‌to‌ ‌correctly‌ ‌identify‌ ‌different‌ ‌objects‌ ‌at‌ ‌various‌ ‌angles‌ ‌and‌ ‌
positions.‌ ‌As‌ ‌seen‌ ‌in‌ ‌Figure‌ ‌8,‌ ‌at‌ ‌a‌ ‌training‌ ‌size‌ ‌of‌ ‌4860,‌ ‌HTM‌ ‌outperformed‌ ‌the‌ ‌
traditional‌ ‌convolutional‌ ‌neural‌ ‌network‌ ‌(Lomonaco‌ ‌&‌ ‌Maloni,‌ ‌2015).‌ ‌ ‌
I‌ ‌applied‌ ‌both‌ ‌of‌ ‌these‌ ‌functions‌ ‌in‌ ‌the‌ ‌proposed‌ ‌model,‌ ‌with‌ ‌the‌ ‌exception‌ ‌that‌ ‌
neural‌ ‌activation‌ ‌is‌ ‌dependent‌ ‌on‌ ‌the‌ ‌‌summation‌ ‌at‌ ‌the‌ ‌‌neuron,‌ ‌rather‌ ‌than‌ ‌‌the‌ ‌number‌ ‌
of‌ ‌active‌ ‌dendritic‌ ‌branches.‌
 ‌
17‌ ‌
Fig.‌ ‌9.‌ ‌Graph‌ ‌of‌ ‌HTM‌ ‌accuracy‌ ‌(blue)‌ ‌vs.‌ ‌LeNet7‌ ‌accuracy‌ ‌(red).‌ ‌
With‌ ‌this‌ ‌being‌ ‌said,‌ ‌alternative‌ ‌applications‌ ‌of‌ ‌existing‌ ‌neuroscience‌ ‌research‌ ‌
have‌ ‌been‌ ‌explored‌ ‌in‌ ‌Miconi,‌ ‌Clune,‌ ‌and‌ ‌Stanley’s‌ ‌“differentiable‌ ‌plasticity”.‌ ‌In‌ ‌their‌ ‌
2018‌ ‌paper,‌ ‌they‌ ‌explore‌ ‌plastic‌ ‌networks‌ ‌through‌ ‌the‌ ‌use‌ ‌of‌ ‌a‌ ‌“Hebbian‌ ‌trace”.‌ ‌This‌ ‌is‌ ‌
a‌ ‌value‌ ‌that‌ ‌is‌ ‌described‌ ‌as‌ ‌“a‌ ‌running‌ ‌average‌ ‌of‌ ‌the‌ ‌product‌ ‌of‌ ‌pre-‌ ‌and‌ ‌post-synaptic‌ ‌
activity”,‌ ‌meaning‌ ‌that‌ ‌this‌ ‌plastic‌ ‌component‌ ‌will‌ ‌change‌ ‌depending‌ ‌on‌ ‌“ongoing‌ ‌inputs‌ ‌
and‌ ‌outputs”.‌ ‌Additionally‌ ‌a‌ ‌plasticity‌ ‌coefficient‌ ‌is‌ ‌used‌ ‌to‌ ‌determine‌ ‌the‌ ‌degree‌ ‌of‌ ‌
plasticity‌ ‌a‌ ‌connection‌ ‌may‌ ‌have,‌ ‌or‌ ‌if‌ ‌that‌ ‌connection‌ ‌will‌ ‌be‌ ‌a‌ ‌fixed‌ ‌value‌ ‌(Miconi,‌ ‌
Clune‌ ‌&‌ ‌Stanley,‌ ‌2018).‌ ‌ ‌
I‌ ‌ended‌ ‌up‌ ‌not‌ ‌using‌ ‌this‌ ‌method‌ ‌to‌ ‌calculate‌ ‌the‌ ‌degree‌ ‌of‌ ‌plasticity‌ ‌in‌ ‌my‌ ‌
network,‌ ‌rather‌ ‌I‌ ‌took‌ ‌inspiration‌ ‌from‌ ‌its‌ ‌effect‌ ‌on‌ ‌the‌ ‌inputs,‌ ‌or‌ ‌neurotransmitter‌ ‌values,‌ ‌
xj(t) .‌ ‌
 ‌
Fig.‌ ‌10.‌ ‌The‌ ‌Hebbian‌ ‌trace‌ ‌(‌Hebb)‌ ‌is‌ ‌updated‌ ‌by‌ ‌a‌ ‌small‌ ‌value‌ ‌(‌η)‌ ‌of‌ ‌the‌ ‌combination‌ ‌of‌ ‌previous‌ ‌input‌ ‌to‌ ‌the‌ ‌neuron‌  ‌(‌
xi(t−1))‌ ‌and‌ ‌current‌ ‌output‌ ‌of‌ ‌the‌ ‌neuron‌ ‌(‌xj(t)).‌ ‌
 ‌
Fig.‌ ‌11.‌ ‌The‌ ‌Hebbian‌ ‌trace‌ ‌is‌ ‌combined‌ ‌with‌ ‌the‌ ‌plasticity‌ ‌coefficient‌ ‌(‌α)‌ ‌to‌ ‌form‌ ‌a‌ ‌plastic‌ ‌component‌ ‌to‌ ‌the‌ ‌input‌ ‌of‌ ‌the‌ ‌
next‌ ‌neuron,‌ ‌xj(t).‌ ‌
 ‌
When‌ ‌shown‌ ‌five‌ ‌sets‌ ‌of‌ ‌50-bit,‌ ‌binary‌ ‌patterns,‌ ‌three‌ ‌types‌ ‌of‌ ‌recurrent‌ ‌neural‌ ‌
networks‌ ‌(RNN)‌ ‌--‌ ‌or‌ ‌networks‌ ‌used‌ ‌for‌ ‌sequential‌ ‌inputs‌ ‌(LeCun,‌ ‌Bengio‌ ‌&‌ ‌Hinton,‌ ‌
18‌ ‌
2015)‌ ‌--‌ ‌had‌ ‌to‌ ‌memorize‌ ‌and‌ ‌predict‌ ‌the‌ ‌next‌ ‌binary‌ ‌string.‌ ‌Differentiable‌ ‌plasticity‌ ‌
solved‌ ‌this‌ ‌problem‌ ‌much‌ ‌quicker‌ ‌than‌ ‌existing‌ ‌recurrent‌ ‌methods‌ ‌could.‌ ‌This‌ ‌data‌ ‌type‌ ‌
was‌ ‌another‌ ‌heavy‌ ‌influence‌ ‌to‌ ‌my‌ ‌model.‌ ‌
 ‌
Fig.‌ ‌12.‌ ‌The‌ ‌Plastic‌ ‌RNN,‌ ‌which‌ ‌utilizes‌ ‌differentiable‌ ‌plasticity,‌ ‌outperforms‌ ‌the‌ ‌LSTM‌ ‌and‌ ‌Non-plastic‌ ‌RNN‌ ‌--‌ ‌both‌ ‌commonplace‌ ‌in‌ ‌
machine‌ ‌learning‌ ‌--‌ ‌in‌ ‌a‌ ‌test‌ ‌of‌ ‌two‌ ‌sets‌ ‌of‌ ‌50-bit,‌ ‌binary‌ ‌patterns.‌ ‌
 ‌
While‌ ‌not‌ ‌considerably‌ ‌more‌ ‌efficient‌ ‌at‌ ‌all‌ ‌times,‌ ‌neuroscience‌ ‌theory‌ ‌has‌ ‌real‌ ‌
applications,‌ ‌and‌ ‌the‌ ‌potential‌ ‌to‌ ‌get‌ ‌increasingly‌ ‌better,‌ ‌even‌ ‌past‌ ‌current‌ ‌methods‌ ‌of‌ ‌
artificial‌ ‌intelligence.‌ ‌
 ‌
Conclusion‌ ‌
As‌ ‌seen‌ ‌in‌ ‌the‌ ‌progression‌ ‌of‌ ‌artificial‌ ‌intelligence,‌ ‌neurological‌ ‌theory‌ ‌has‌ ‌ ‌
played‌ ‌a‌ ‌large‌ ‌factor‌ ‌in‌ ‌the‌ ‌success‌ ‌of‌ ‌current‌ ‌day‌ ‌algorithms.‌ ‌Therefore,‌ ‌it‌ ‌is‌ ‌essential‌ ‌
to‌ ‌research‌ ‌new‌ ‌ways‌ ‌of‌ ‌applying‌ ‌thoroughly-studied‌ ‌neuroscience‌ ‌research‌ ‌to‌ ‌the‌ ‌
emerging‌ ‌field‌ ‌of‌ ‌AI.‌ ‌In‌ ‌theory,‌ ‌it‌ ‌should‌ ‌improve‌ ‌accuracy,‌ ‌and‌ ‌by‌ ‌extension,‌ ‌the‌ ‌
“intelligence”‌ ‌of‌ ‌our‌ ‌computers‌ ‌‌—‌ ‌especially‌ ‌since‌ ‌there‌ ‌is‌ ‌hard‌ ‌evidence‌ ‌of‌ ‌neocortical‌ ‌
19‌ ‌
and‌ ‌plasticity-based‌ ‌theories‌ ‌improving‌ ‌upon‌ ‌modern‌ ‌methods‌ ‌of‌ ‌AI.‌ ‌Despite‌ ‌the‌ ‌
optimized‌ ‌algorithms‌ ‌that‌ ‌seemingly‌ ‌run‌ ‌our‌ ‌world‌ ‌adequately,‌ ‌it‌ ‌is‌ ‌important‌ ‌to‌ ‌explore‌ ‌
new‌ ‌and‌ ‌exciting‌ ‌avenues‌ ‌of‌ ‌artificial‌ ‌intelligence,‌ ‌where‌ ‌machine‌ ‌learning‌ ‌may‌ ‌not‌ ‌be‌ ‌
the‌ ‌sole‌ ‌solution.‌ ‌In‌ ‌the‌ ‌words‌ ‌of‌ ‌philosopher‌ ‌Thomas‌ ‌Nagel,‌ ‌“too‌ ‌much‌ ‌time‌ ‌is‌ ‌wasted‌ ‌
because‌ ‌of‌ ‌the‌ ‌assumption‌ ‌that‌ ‌methods‌ ‌already‌ ‌in‌ ‌existence‌ ‌will‌ ‌solve‌ ‌problems‌ ‌for‌ ‌
which‌ ‌they‌ ‌were‌ ‌not‌ ‌designed”‌ ‌(Brody,‌ ‌2013;‌ ‌Hahlweg‌ ‌&‌ ‌Hooker,‌ ‌et.‌ ‌al.,‌ ‌1989).‌ ‌No‌ ‌
current‌ ‌theories‌ ‌narrowly‌ ‌examine‌ ‌artificial‌ ‌plasticity’s‌ ‌effect‌ ‌on‌ ‌the‌ ‌accuracy‌ ‌of‌ ‌
computer‌ ‌algorithms,‌ ‌when‌ ‌applied‌ ‌to‌ ‌biologically-determined‌ ‌rules‌ ‌of‌ ‌connectivity.‌ ‌How‌ ‌
do‌‌ ‌the‌ ‌principles‌ ‌of‌ ‌neural‌ ‌connectivity‌ ‌and‌ ‌neuroplasticity‌ ‌affect‌ ‌the‌ ‌accuracy‌ ‌of‌ ‌
artificial‌ ‌neural‌ ‌networks‌ ‌on‌ ‌the‌ ‌recognition‌ ‌of‌ ‌binary‌ ‌patterns?‌ ‌
 ‌
Methodology‌ ‌
Experimental‌ ‌Design‌ ‌
In‌ ‌order‌ ‌to‌ ‌best‌ ‌answer‌ ‌this‌ ‌question,‌ ‌I‌ ‌utilized‌ ‌a‌ ‌true‌ ‌experimental‌ ‌study.‌ ‌Since‌ ‌ ‌
each‌ ‌artificial‌ ‌neural‌ ‌network‌ ‌algorithm‌ ‌is‌ ‌hard-coded,‌ ‌they‌ ‌will‌ ‌not‌ ‌vary‌ ‌from‌ ‌post‌ ‌to‌ ‌
pretest‌ ‌if‌ ‌given‌ ‌the‌ ‌same‌ ‌data;‌ ‌therefore,‌ ‌I‌ ‌have‌ ‌chosen‌ ‌to‌ ‌perform‌ ‌a‌ ‌posttest‌ ‌only‌ ‌
design,‌ ‌where‌ ‌the‌ ‌experimental‌ ‌group‌ ‌is‌ ‌given‌ ‌a‌ ‌treatment‌ ‌and‌ ‌tested‌ ‌alongside‌ ‌the‌ ‌
control‌ ‌group‌ ‌(Insights‌ ‌Association).‌ ‌For‌ ‌this‌ ‌experiment,‌ ‌I‌ ‌decided‌ ‌to‌ ‌use‌ ‌quantitative‌ ‌
data‌ ‌to‌ ‌determine‌ ‌the‌ ‌accuracy‌ ‌of‌ ‌both‌ ‌networks,‌ ‌since‌ ‌both‌ ‌algorithms‌ ‌output‌ ‌a‌ ‌value‌ ‌
representing‌ ‌their‌ ‌degree‌ ‌of‌ ‌error‌ ‌every‌ ‌one‌ ‌hundred‌ ‌iterations.‌ ‌Additionally,‌ ‌I‌ ‌am‌ ‌
utilizing‌ ‌a‌ ‌binary‌ ‌classifier‌ ‌neural‌ ‌network‌ ‌for‌ ‌my‌ ‌data,‌ ‌which‌ ‌means‌ ‌that‌ ‌each‌ ‌output‌ ‌will‌ ‌
return‌ ‌a‌ ‌prediction‌ ‌of‌ ‌zero‌ ‌or‌ ‌one,‌ ‌in‌ ‌order‌ ‌to‌ ‌distinguish‌ ‌between‌ ‌two‌ ‌classes‌ ‌of‌ ‌data.‌ ‌
20‌ ‌
Binary‌ ‌classification‌ ‌is‌ ‌widely‌ ‌used‌ ‌for‌ ‌classification‌ ‌problems‌ ‌(‌Jiawei‌ ‌Han,‌ ‌et.‌ ‌al,‌ ‌2012),‌ ‌
such‌ ‌as‌ ‌sentiment‌ ‌analysis‌ ‌and‌ ‌image‌ ‌classification‌ ‌(Jeremy‌ ‌Howard,‌ ‌2019),‌ ‌but‌ ‌it‌ ‌is‌ ‌
also‌ ‌a‌ ‌task‌ ‌that‌ ‌is‌ ‌simple‌ ‌to‌ ‌implement‌ ‌given‌ ‌time‌ ‌constraints.‌ ‌I‌ ‌will‌ ‌also‌ ‌be‌ ‌following‌ ‌a‌ ‌
“supervised‌ ‌learning”‌ ‌approach,‌ ‌meaning‌ ‌that‌ ‌all‌ ‌data‌ ‌will‌ ‌have‌ ‌some‌ ‌label‌ ‌(LeCun,‌ ‌
Bengio‌ ‌&‌ ‌Hinton,‌ ‌2015)‌ ‌(either‌ ‌a‌ ‌zero‌ ‌or‌ ‌a‌ ‌one‌ ‌in‌ ‌my‌ ‌case),‌ ‌which‌ ‌will‌ ‌make‌ ‌the‌ ‌training‌ ‌
of‌ ‌the‌ ‌network‌ ‌much‌ ‌more‌ ‌efficient.‌ ‌
The‌ ‌data‌ ‌used‌ ‌in‌ ‌this‌ ‌experiment‌ ‌consists‌ ‌of‌ ‌256‌ ‌8-bit‌ ‌binary‌ ‌sequences‌ ‌--‌ ‌191‌ ‌ ‌
and‌ ‌65‌ ‌in‌ ‌the‌ ‌training‌ ‌and‌ ‌testing‌ ‌sets‌ ‌respectively.‌ ‌Each‌ ‌bit‌ ‌in‌ ‌a‌ ‌sequence‌ ‌will‌ ‌be‌ ‌fed‌ ‌
into‌ ‌the‌ ‌network‌ ‌as‌ ‌its‌ ‌own‌ ‌input;‌ ‌in‌ ‌order‌ ‌to‌ ‌classify‌ ‌each‌ ‌sequence,‌ ‌I‌ ‌will‌ ‌apply‌ ‌some‌ ‌
arbitrary‌ ‌rule‌ ‌to‌ ‌each‌ ‌sequence‌ ‌in‌ ‌the‌ ‌dataset‌ ‌(“1”‌ ‌must‌ ‌be‌ ‌the‌ ‌first‌ ‌bit‌ ‌position,‌ ‌“0”‌ ‌must‌ ‌
be‌ ‌in‌ ‌the‌ ‌second‌ ‌and‌ ‌third‌ ‌bit‌ ‌positions,‌ ‌etc),‌ ‌forcing‌ ‌the‌ ‌network‌ ‌to‌ ‌accurately‌ ‌identify‌ ‌a‌ ‌
pattern‌ ‌and‌ ‌use‌ ‌its‌ ‌identification‌ ‌to‌ ‌make‌ ‌further‌ ‌correct‌ ‌predictions.‌ ‌I‌ ‌felt‌ ‌comfortable‌ ‌
assessing‌ ‌the‌ ‌accuracy‌ ‌of‌ ‌classification‌ ‌abilities‌ ‌of‌ ‌artificial‌ ‌neural‌ ‌networks‌ ‌on‌ ‌this‌ ‌
system,‌ ‌since‌ ‌differentiable‌ ‌plasticity‌ ‌also‌ ‌used‌ ‌multi-bit‌ ‌representations‌ ‌as‌ ‌input;‌ ‌the‌ ‌
difference‌ ‌is‌ ‌that‌ ‌they‌ ‌tested‌ ‌for‌ ‌prediction‌ ‌of‌ ‌the‌ ‌next‌ ‌binary‌ ‌pattern‌ ‌in‌ ‌a‌ ‌sequence‌ ‌
(Miconi,‌ ‌Clune‌ ‌&‌ ‌Stanley,‌ ‌2018),‌ ‌while‌ ‌I‌ ‌am‌ ‌testing‌ ‌for‌ ‌classification‌ ‌of‌ ‌a‌ ‌binary‌ ‌pattern‌ ‌
with‌ ‌a‌ ‌fixed‌ ‌rule.‌ ‌Additionally,‌ ‌I‌ ‌found‌ ‌that‌ ‌the‌ ‌type‌ ‌of‌ ‌rule‌ ‌did‌ ‌not‌ ‌matter,‌ ‌as‌ ‌long‌ ‌as‌ ‌it‌ ‌
was‌ ‌only‌ ‌applied‌ ‌to‌ ‌two‌ ‌bit‌ ‌positions.‌ ‌For‌ ‌both‌ ‌algorithms,‌ ‌the‌ ‌rule‌ ‌was‌ ‌“0”‌ ‌in‌ ‌the‌ ‌fourth‌ ‌
place,‌ ‌and‌ ‌a‌ ‌“1”‌ ‌in‌ ‌the‌ ‌sixth‌ ‌place.‌ ‌
21‌ ‌
 ‌
Fig.‌ ‌13.‌ ‌Visualization‌ ‌of‌ ‌my‌ ‌deep‌ ‌artificial‌ ‌neural‌ ‌network‌ ‌using‌ ‌NN-SVG.‌ ‌
 ‌
The‌ ‌neural‌ ‌network‌ ‌that‌ ‌I‌ ‌will‌ ‌be‌ ‌using‌ ‌has‌ ‌the‌ ‌dimensions‌ ‌ ‌
8x8x8x1,‌ ‌as‌ ‌seen‌ ‌in‌ ‌Figure‌ ‌13.‌ ‌Since‌ ‌there‌ ‌are‌ ‌no‌ ‌strict‌ ‌rules‌ ‌for‌ ‌the‌ ‌shape‌ ‌of‌ ‌a‌ ‌neural‌ ‌
network‌ ‌on‌ ‌a‌ ‌given‌ ‌problem,‌ ‌my‌ ‌decision‌ ‌was‌ ‌made‌ ‌for‌ ‌two‌ ‌reasons:‌ ‌the‌ ‌data‌ ‌requires‌ ‌
eight‌ ‌separate‌ ‌input‌ ‌positions‌ ‌for‌ ‌each‌ ‌bit,‌ ‌and‌ ‌the‌ ‌more‌ ‌connections‌ ‌--‌ ‌136‌ ‌in‌ ‌total‌ ‌--‌ ‌
the‌ ‌more‌ ‌opportunities‌ ‌to‌ ‌apply‌ ‌each‌ ‌biologically-derived‌ ‌function.‌ ‌
 ‌
Machine‌ ‌Learning‌ ‌Theory‌ ‌and‌ ‌Mathematics‌ ‌
Feedforward‌ ‌networks‌ ‌“are‌ ‌the‌ ‌quintessential‌ ‌deep‌ ‌learning‌ ‌models”,‌ ‌according‌ ‌ ‌
to‌ ‌GAN‌ ‌inventor,‌ ‌Ian‌ ‌Goodfellow,‌ ‌Turing‌ ‌Award‌ ‌winner,‌ ‌Yoshua‌ ‌Bengio,‌ ‌and‌ ‌GAN‌ ‌
co-author,‌ ‌Aaron‌ ‌Courtville.‌ ‌These‌ ‌networks‌ ‌form‌ ‌the‌ ‌basis‌ ‌for‌ ‌modern‌ ‌object‌ ‌
recognition‌ ‌and‌ ‌natural‌ ‌language‌ ‌(Goodfellow,‌ ‌Bengio‌ ‌&‌ ‌Courtville,‌ ‌2016;‌ ‌Goodfellow,‌ ‌
et.‌ ‌al.,‌ ‌2014;‌ ‌Bengio).‌ ‌In‌ ‌order‌ ‌to‌ ‌present‌ ‌an‌ ‌accurate‌ ‌and‌ ‌unvarying‌ ‌mathematical‌ ‌
22‌ ‌
representation‌ ‌of‌ ‌machine‌ ‌learning,‌ ‌the‌ ‌following‌ ‌information‌ ‌will‌ ‌reflect‌ ‌Stanford’s‌ ‌CS‌ ‌
229‌ ‌-‌ ‌Machine‌ ‌Learning‌ ‌course.‌ ‌It‌ ‌is‌ ‌necessary‌ ‌to‌ ‌have‌ ‌an‌ ‌understanding‌ ‌of‌ ‌these‌ ‌
functions,‌ ‌because‌ ‌I‌ ‌will‌ ‌be‌ ‌applying‌ ‌my‌ ‌own‌ ‌biologically-derived‌ ‌functions‌ ‌that‌ ‌will‌ ‌
reference‌ ‌them.‌ ‌
In‌ ‌Figure‌ ‌14,‌ ‌the‌ ‌variable‌ ‌x ‌acts‌ ‌as‌ ‌data‌ ‌input‌ ‌into‌ ‌a‌ ‌neural‌ ‌network;‌ ‌it‌ ‌could‌ ‌also‌ ‌ ‌
be‌ ‌thought‌ ‌of‌ ‌as‌ ‌the‌ ‌neurotransmitters.‌ ‌This‌ ‌input‌ ‌value‌ ‌is‌ ‌then‌ ‌assigned‌ ‌a‌ ‌weight‌ ‌value,‌ ‌
(W),‌ ‌which‌ ‌acts‌ ‌as‌ ‌a‌ ‌connection‌ ‌between‌ ‌neurons;‌ ‌it‌ ‌can‌ ‌also‌ ‌represent‌ ‌the‌ ‌degree‌ ‌of‌ ‌
depolarization‌ ‌in‌ ‌a‌ ‌neuron.‌ ‌Additionally,‌ ‌a‌ ‌bias‌ ‌b  ‌is‌ ‌added‌ ‌to‌ ‌the‌ ‌product‌ ‌of‌ ‌the‌ ‌weight‌ ‌
and‌ ‌input.‌ ‌This‌ ‌is‌ ‌important,‌ ‌since‌ ‌the‌ ‌bias‌ ‌can‌ ‌be‌ ‌thought‌ ‌of‌ ‌as‌ ‌a‌ ‌y-intercept‌ ‌value,‌ ‌
necessary‌ ‌for‌ ‌an‌ ‌accurate‌ ‌linear‌ ‌model;‌ ‌you‌ ‌can‌ ‌think‌ ‌of‌ ‌Figure‌ ‌14‌ ‌as‌ ‌a‌ ‌y=mx+b  ‌
graph‌ ‌(PICO).‌ ‌These‌ ‌propagated‌ ‌z ‌values,‌ ‌as‌ ‌seen‌ ‌in‌ ‌Figure‌ ‌14,‌ ‌are‌ ‌summed‌ ‌at‌ ‌each‌ ‌
neuron‌ ‌and‌ ‌an‌ ‌activation‌ ‌function‌ ‌is‌ ‌applied.‌ ‌ ‌
 ‌
Fig.‌ ‌14.‌ ‌Forward‌ ‌propagation.‌ ‌
 ‌
Sigmoid‌ ‌is‌ ‌a‌ ‌common‌ ‌activation‌ ‌function‌ ‌that‌ ‌squashes‌ ‌a‌ ‌value‌ ‌between‌ ‌zero‌ ‌
and‌ ‌one‌ ‌to‌ ‌prevent‌ ‌values‌ ‌from‌ ‌becoming‌ ‌exponentially‌ ‌large,‌ ‌but‌ ‌it‌ ‌can‌ ‌also‌ ‌be‌ ‌thought‌ ‌
of‌ ‌as‌ ‌a‌ ‌function‌ ‌that‌ ‌converts‌ ‌a‌ ‌signal‌ ‌to‌ ‌neurotransmitters;‌ ‌I‌ ‌will‌ ‌use‌ ‌this‌ ‌function‌ ‌in‌ ‌the‌ ‌
final‌ ‌layer‌ ‌of‌ ‌my‌ ‌neural‌ ‌network‌ ‌(Figure‌ ‌15)‌ ‌to‌ ‌provide‌ ‌a‌ ‌binary‌ ‌output.‌ ‌Tanh‌ ‌is‌ ‌similar,‌ ‌
except‌ ‌values‌ ‌lie‌ ‌between‌ ‌negative‌ ‌one‌ ‌and‌ ‌one‌ ‌(Figure‌ ‌16);‌ ‌this‌ ‌function‌ ‌will‌ ‌be‌ ‌used‌ ‌
for‌ ‌the‌ ‌remainder‌ ‌of‌ ‌the‌ ‌network’s‌ ‌layers.‌ ‌
23‌ ‌
 ‌
Fig.‌ ‌15.‌ ‌Sigmoid‌ ‌activation‌ ‌function‌ ‌
 ‌
Fig.‌ ‌16.‌ ‌Tanh‌ ‌activation‌ ‌function.‌ ‌
 ‌
The‌ ‌output‌ ‌of‌ ‌these‌ ‌functions‌ ‌should‌ ‌equal‌ ‌a‌ ‌target‌ ‌value,‌ ‌y,‌ ‌but‌ ‌to‌ ‌find‌ ‌how‌ ‌
close‌ ‌the‌ ‌actual‌ ‌output‌ ‌is‌ ‌to‌ ‌the‌ ‌expected‌ ‌output,‌ ‌a‌ ‌cost‌ ‌function‌ ‌must‌ ‌be‌ ‌applied‌ ‌(Figure‌ ‌
17);‌ ‌this‌ ‌calculated‌ ‌value‌ ‌is‌ ‌referred‌ ‌to‌ ‌as‌ ‌“loss”.‌ ‌ ‌
 ‌
Fig.‌ ‌17.‌ ‌Cross-entropy‌ ‌loss‌ ‌function.‌ ‌
 ‌
The‌ ‌new‌ ‌error‌ ‌value‌ ‌can‌ ‌then‌ ‌be‌ ‌used‌ ‌for‌ ‌gradient‌ ‌descent‌ ‌where‌ ‌loss‌ ‌is‌ ‌
minimized‌ ‌by‌ ‌updating‌ ‌the‌ ‌weight‌ ‌values‌ ‌(Figure‌ ‌18).‌ ‌incrementally‌ ‌and‌ ‌optimally.‌ ‌Over‌ ‌
time,‌ ‌through‌ ‌many‌ ‌iterations,‌ ‌the‌ ‌neural‌ ‌network‌ ‌should‌ ‌begin‌ ‌to‌ ‌produce‌ ‌more‌ ‌
accurate‌ ‌outputs‌ ‌(Ng,‌ ‌2018;‌ ‌Amidi‌ ‌&‌ ‌Amidi,‌ ‌2018).‌ ‌ ‌
 ‌
Fig.‌ ‌18.‌ ‌Gradient‌ ‌Descent.‌ ‌
 ‌
24‌ ‌
It‌ ‌is‌ ‌important‌ ‌to‌ ‌understand‌ ‌these‌ ‌equations,‌ ‌since‌ ‌they‌ ‌will‌ ‌be‌ ‌used‌ ‌in‌ ‌both‌ ‌the‌ ‌
controlled‌ ‌and‌ ‌manipulated‌ ‌algorithms;‌ ‌they‌ ‌will‌ ‌coexist‌ ‌with‌ ‌the‌ ‌biological‌ ‌equations.‌ ‌
 ‌
 ‌
Justification‌ ‌of‌ ‌Method‌ ‌
My‌ ‌experiment‌ ‌sets‌ ‌itself‌ ‌apart‌ ‌from‌ ‌similar‌ ‌studies,‌ ‌such‌ ‌as‌ ‌Numenta’s‌ ‌HTM‌ ‌ ‌
theory‌ ‌and‌ ‌differential‌ ‌plasticity,‌ ‌in‌ ‌a‌ ‌number‌ ‌of‌ ‌ways.‌ ‌Numenta‌ ‌has‌ ‌three‌ ‌main‌ ‌focuses:‌ ‌
cortical‌ ‌columns‌ ‌--‌ ‌finding‌ ‌a‌ ‌framework‌ ‌for‌ ‌the‌ ‌hierarchical‌ ‌structure‌ ‌of‌ ‌biological‌ ‌cortical‌ ‌
columns‌ ‌that‌ ‌form‌ ‌the‌ ‌cortex‌ ‌--‌ ‌sequence‌ ‌learning‌ ‌--‌ ‌a‌ ‌study‌ ‌of‌ ‌how‌ ‌neurons‌ ‌can‌ ‌make‌ ‌
accurate‌ ‌predictions‌ ‌over‌ ‌a‌ ‌large‌ ‌sequence‌ ‌of‌ ‌data‌ ‌over‌ ‌time‌ ‌--‌ ‌and‌ ‌sparse‌ ‌distributed‌ ‌
representations‌ ‌--‌ ‌sparse‌ ‌neuron‌ ‌representation‌ ‌(Numenta).‌ ‌These‌ ‌research‌ ‌areas‌ ‌
require‌ ‌some‌ ‌properties‌ ‌associated‌ ‌with‌ ‌neural‌ ‌connectivity‌ ‌and‌ ‌plasticity‌ ‌(Figure‌ ‌7‌ ‌and‌ ‌
Figure‌ ‌8),‌ ‌but‌ ‌these‌ ‌algorithms‌ ‌are‌ ‌not‌ ‌the‌ ‌direct‌ ‌focus‌ ‌of‌ ‌their‌ ‌experiments,‌ ‌rather‌ ‌they‌ ‌
are‌ ‌tools‌ ‌used‌ ‌to‌ ‌accomplish‌ ‌much‌ ‌broader‌ ‌goals.‌ ‌I‌ ‌have‌ ‌taken‌ ‌inspiration‌ ‌from‌ ‌their‌ ‌
interpretation‌ ‌of‌ ‌an‌ ‌artificial‌ ‌action‌ ‌potential‌ ‌and‌ ‌artificial‌ ‌long-term‌ ‌potentiation‌ ‌and‌ ‌
depression,‌ ‌but‌ ‌have‌ ‌implemented‌ ‌a‌ ‌novel‌ ‌algorithm,‌ ‌since‌ ‌my‌ ‌question‌ ‌is‌ ‌much‌ ‌more‌ ‌
narrowed‌ ‌on‌ ‌plasticity‌ ‌and‌ ‌interactions‌ ‌between‌ ‌individual‌ ‌neurons.‌ ‌In‌ ‌order‌ ‌to‌ ‌properly‌ ‌
carry‌ ‌out‌ ‌these‌ ‌principles,‌ ‌I‌ ‌felt‌ ‌as‌ ‌if‌ ‌it‌ ‌was‌ ‌necessary‌ ‌to‌ ‌focus‌ ‌on‌ ‌the‌ ‌role‌ ‌of‌ ‌
neurotransmitters,‌ ‌receptors,‌ ‌and‌ ‌homeostatic‌ ‌plasticity,‌ ‌which‌ ‌are‌ ‌all‌ ‌beyond‌ ‌the‌ ‌focus‌ ‌
of‌ ‌HTM‌ ‌models.‌ ‌
Similarly,‌ ‌differentiable‌ ‌plasticity‌ ‌influenced‌ ‌my‌ ‌application‌ ‌of‌ ‌plasticity,‌ ‌but‌ ‌fails‌ ‌to‌ ‌
dive‌ ‌beyond‌ ‌Hebbian‌ ‌plasticity‌ ‌or‌ ‌address‌ ‌biological‌ ‌neural‌ ‌connectivity.‌ ‌
25‌ ‌
Both‌ ‌Numenta‌ ‌and‌ ‌differentiable‌ ‌plasticity‌ ‌have‌ ‌their‌ ‌pros‌ ‌and‌ ‌cons:‌ ‌a‌ ‌more‌ ‌
accurate‌ ‌neocortical‌ ‌theory,‌ ‌but‌ ‌a‌ ‌broader‌ ‌focus‌ ‌and‌ ‌a‌ ‌general,‌ ‌Hebbian-based‌ ‌theory‌ ‌
of‌ ‌neuroscience,‌ ‌without‌ ‌a‌ ‌thorough‌ ‌focus‌ ‌on‌ ‌plasticity,‌ ‌respectively.‌ ‌This‌ ‌is‌ ‌why‌ ‌I‌ ‌have‌ ‌
taken‌ ‌inspiration‌ ‌from‌ ‌both‌ ‌ideas‌ ‌in‌ ‌order‌ ‌to‌ ‌answer‌ ‌my‌ ‌question‌ ‌with‌ ‌the‌ ‌greatest‌ ‌
accuracy.‌ ‌My‌ ‌experiment‌ ‌is‌ ‌a‌ ‌corroboration‌ ‌of‌ ‌information‌ ‌from‌ ‌Numenta,‌ ‌differentiable‌ ‌
plasticity,‌ ‌and‌ ‌modern‌ ‌neuroscience‌ ‌research.‌ ‌ ‌
 ‌
Biologically-Derived‌ ‌Equations‌ ‌and‌ ‌Implementation‌ ‌
As‌ ‌the‌ ‌name‌ ‌suggests,‌ ‌artificial‌ ‌neural‌ ‌networks‌ ‌are‌ ‌based‌ ‌on‌ ‌their‌ ‌biological‌ ‌ ‌
counterparts.‌ ‌Therefore,‌ ‌in‌ ‌order‌ ‌to‌ ‌effectively‌ ‌apply‌ ‌artificial‌ ‌neural‌ ‌connectivity‌ ‌and‌ ‌
plasticity,‌ ‌I‌ ‌needed‌ ‌to‌ ‌use‌ ‌existing‌ ‌machine‌ ‌learning‌ ‌symbolism,‌ ‌and‌ ‌pair‌ ‌it‌ ‌to‌ ‌existing‌ ‌
biological‌ ‌features.‌ ‌
The‌ ‌first‌ ‌equation‌ ‌(Figure‌ ‌20)‌ ‌regards‌ ‌the‌ ‌activation‌ ‌of‌ ‌a‌ ‌specific‌ ‌neuron.‌ ‌The‌ ‌
∑  (z) ‌value‌ ‌represents‌ ‌summation‌ ‌of‌ ‌ions‌ ‌in‌ ‌the‌ ‌membrane‌ ‌that‌ ‌may‌ ‌incite‌ ‌an‌ ‌activation‌ ‌
if‌ ‌it‌ ‌exceeds‌ ‌a‌ ‌threshold‌ ‌θ′ ,‌ ‌otherwise‌ ‌it‌ ‌will‌ ‌become‌ ‌zero,‌ ‌effectively‌ ‌“turning‌ ‌off”‌ ‌that‌ ‌
neuron’s‌ ‌signal.‌ ‌This‌ ‌threshold‌ ‌has‌ ‌been‌ ‌tuned‌ ‌to‌ ‌5‌ ‌in‌ ‌order‌ ‌to‌ ‌promote‌ ‌greater‌ ‌sparsity‌ ‌
in‌ ‌my‌ ‌implementation.‌ ‌
 ‌
Fig.‌ ‌20.‌ ‌Activation‌ ‌potential‌ ‌equation.‌ ‌
 ‌
26‌ ‌
The‌ ‌second‌ ‌equation‌ ‌(Figure‌ ‌21)‌ ‌considers‌ ‌the‌ ‌neurotransmitters,‌ ‌represented‌ ‌
by‌ ‌the‌ ‌symbol‌ ‌a,‌ ‌that‌ ‌cross‌ ‌the‌ ‌synapse.‌ ‌In‌ ‌order‌ ‌to‌ ‌factor‌ ‌in‌ ‌restrictions‌ ‌on‌ ‌the‌ ‌number‌ ‌
of‌ ‌neurotransmitters‌ ‌that‌ ‌are‌ ‌received‌ ‌by‌ ‌receptors,‌ ‌which‌ ‌would‌ ‌biologically‌ ‌come‌ ‌in‌ ‌
the‌ ‌form‌ ‌of‌ ‌diffusion,‌ ‌enzymatic‌ ‌degradation,‌ ‌reuptake,‌ ‌or‌ ‌glial‌ ‌cells,‌ ‌these‌ ‌a ‌values‌ ‌are‌ ‌
restricted‌ ‌by‌ ‌the‌ ‌number‌ ‌of‌ ‌receptors,‌ ‌R,‌ ‌at‌ ‌a‌ ‌given‌ ‌synapse.‌ ‌Receptors‌ ‌are‌ ‌initialized‌ ‌
at‌ ‌a‌ ‌value‌ ‌of‌ ‌0.35‌ ‌
 ‌
Fig.‌ ‌21.‌ ‌Neurotransmitter‌ ‌equation.‌ ‌
 ‌
In‌ ‌the‌ ‌third‌ ‌equation‌ ‌(Figure‌ ‌22),‌ ‌synapses‌ ‌are‌ ‌strengthened‌ ‌or‌ ‌weakened‌ ‌
depending‌ ‌on‌ ‌their‌ ‌activation.‌ ‌Therefore,‌ ‌if‌ ‌the‌ ‌first‌ ‌equation‌ ‌allows‌ ‌an‌ ‌action‌ ‌potential,‌ ‌
neurotransmitters‌ ‌will‌ ‌be‌ ‌sent‌ ‌over‌ ‌a‌ ‌synapse‌ ‌and‌ ‌received‌ ‌by‌ ‌receptors.‌ ‌Over‌ ‌many‌ ‌
iterations‌ ‌receptors‌ ‌on‌ ‌the‌ ‌receiving‌ ‌neuron‌ ‌increase‌ ‌or‌ ‌decrease‌ ‌depending‌ ‌on‌ ‌the‌ ‌
activation‌ ‌of‌ ‌the‌ ‌previous‌ ‌neuron.‌ ‌This‌ ‌process‌ ‌is‌ ‌represented‌ ‌by‌ ‌a‌ ‌slight‌ ‌increase‌ ‌(‌nP)‌ ‌
or‌ ‌decrease‌ ‌(‌nD)‌ ‌to‌ ‌the‌ ‌R ‌value.‌ ‌Potentiation‌ ‌and‌ ‌depression‌ ‌constants‌ ‌are‌ ‌set‌ ‌to‌ ‌
0.0125‌ ‌and‌ ‌-0.0045‌ ‌respectively,‌ ‌not‌ ‌unlike‌ ‌Numenta’s‌ ‌values‌ ‌of‌ ‌0.015‌ ‌and‌ ‌-0.0025.‌ ‌
Also,‌ ‌negative‌ ‌receptors‌ ‌do‌ ‌not‌ ‌exist,‌ ‌so‌ ‌the‌ ‌minimum‌ ‌value‌ ‌will‌ ‌always‌ ‌be‌ ‌zero.‌ ‌
27‌ ‌
 ‌
Fig.‌ ‌22.‌ ‌Long‌ ‌term‌ ‌potentiation‌ ‌and‌ ‌depression‌ ‌equation.‌ ‌
 ‌
The‌ ‌final‌ ‌equation‌ ‌(Figure‌ ‌23)‌ ‌addresses‌ ‌homeostatic‌ ‌plasticity.‌ ‌In‌ ‌short,‌ ‌if‌ ‌the‌ ‌
strongest‌ ‌synapse‌ ‌in‌ ‌a‌ ‌neuron‌ ‌exceeds‌ ‌some‌ ‌threshold‌ ‌θ′′ ,‌ ‌then‌ ‌it‌ ‌will‌ ‌be‌ ‌scaled‌ ‌slowly‌ ‌
over‌ ‌some‌ ‌timescale‌ ‌(‌δ),‌ ‌which‌ ‌has‌ ‌been‌ ‌initialized‌ ‌to‌ ‌0.05.‌ ‌
 ‌
Fig.‌ ‌23.‌ ‌Homeostatic‌ ‌plasticity‌ ‌equation.‌ ‌
 ‌
To‌ ‌visualize‌ ‌the‌ ‌relationship‌ ‌between‌ ‌neurotransmitters‌ ‌and‌ ‌receptors,‌ ‌Figure‌ ‌24‌ ‌
illustrates‌ ‌an‌ ‌example‌ ‌of‌ ‌a‌ ‌neural‌ ‌network‌ ‌with‌ ‌both‌ ‌variables‌ ‌in‌ ‌play,‌ ‌versus‌ ‌a‌ ‌standard‌ ‌
network.‌ ‌
28‌ ‌
 ‌
Fig.‌ ‌24.‌ ‌ ‌
 ‌
The‌ ‌controlled‌ ‌neural‌ ‌network‌ ‌without‌ ‌any‌ ‌biological‌ ‌elements‌ ‌can‌ ‌be‌ ‌seen‌ ‌in‌ ‌
Appendix‌ ‌I.‌ ‌All‌ ‌biological‌ ‌equations,‌ ‌as‌ ‌well‌ ‌as‌ ‌each‌ ‌initialized‌ ‌value,‌ ‌can‌ ‌be‌ ‌seen‌ ‌in‌ ‌
Appendix‌ ‌II.‌ ‌
 ‌
Results‌ ‌and‌ ‌Analysis‌ ‌
‌After‌ ‌training‌ ‌on‌ ‌the‌ ‌8-bit‌ ‌data,‌ ‌there‌ ‌was‌ ‌a‌ ‌clear‌ ‌difference‌ ‌in‌ ‌each‌ ‌neural‌ ‌
network’s‌ ‌success‌ ‌in‌ ‌finding‌ ‌a‌ ‌pattern‌ ‌amongst‌ ‌the‌ ‌binary‌ ‌strings.‌ ‌While‌ ‌the‌ ‌cost‌ ‌value‌ ‌
of‌ ‌the‌ ‌controlled‌ ‌algorithm‌ ‌stood‌ ‌at‌ ‌0.000783,‌ ‌the‌ ‌manipulated‌ ‌algorithm‌ ‌had‌ ‌a‌ ‌cost‌ ‌of‌ ‌
0.000368,‌ ‌less‌ ‌than‌ ‌half‌ ‌of‌ ‌the‌ ‌original.‌ ‌
29‌ ‌
 ‌
Fig.‌ ‌25.‌ ‌Controlled‌ ‌neural‌ ‌network‌ ‌training.‌ ‌
 ‌
Fig.‌ ‌26.‌ ‌Manipulated‌ ‌neural‌ ‌network‌ ‌training.‌ ‌
 ‌
When‌ ‌tested‌ ‌on‌ ‌the‌ ‌testing‌ ‌data,‌ ‌the‌ ‌original‌ ‌neural‌ ‌network‌ ‌scored‌ ‌100%‌ ‌
accuracy;‌ ‌however,‌ ‌because‌ ‌of‌ ‌a‌ ‌number‌ ‌of‌ ‌errors‌ ‌in‌ ‌the‌ ‌manipulated‌ ‌testing‌ ‌function‌ ‌
30‌ ‌
and‌ ‌time‌ ‌constraints,‌ ‌I‌ ‌was‌ ‌unable‌ ‌to‌ ‌test‌ ‌the‌ ‌manipulated‌ ‌neural‌ ‌network.‌ ‌Still,‌ ‌based‌ ‌
on‌ ‌its‌ ‌success‌ ‌in‌ ‌terms‌ ‌of‌ ‌training‌ ‌accuracy‌ ‌and‌ ‌efficiency‌ ‌--‌ ‌less‌ ‌cost‌ ‌in‌ ‌fewer‌ ‌iterations‌ ‌
--‌ ‌and‌ ‌100%‌ ‌accuracy‌ ‌of‌ ‌previous‌ ‌manipulated‌ ‌models,‌ ‌I‌ ‌have‌ ‌no‌ ‌doubt‌ ‌that‌ ‌it‌ ‌would‌ ‌
have‌ ‌received‌ ‌a‌ ‌perfect‌ ‌score.‌ ‌
No‌ ‌statistical‌ ‌test‌ ‌was‌ ‌required‌ ‌in‌ ‌order‌ ‌to‌ ‌evaluate‌ ‌these‌ ‌results,‌ ‌since‌ ‌the‌ ‌
aforementioned‌ ‌cost‌ ‌function‌ ‌performs‌ ‌this‌ ‌operation‌ ‌by‌ ‌using‌ ‌cross-entropy‌ ‌loss.‌ ‌
Therefore,‌ ‌the‌ ‌effectiveness‌ ‌of‌ ‌each‌ ‌algorithm‌ ‌is‌ ‌embedded‌ ‌in‌ ‌their‌ ‌code.‌ ‌
 ‌
Limitations‌ ‌
Although‌ ‌the‌ ‌biologically-modeled‌ ‌artificial‌ ‌neural‌ ‌network‌ ‌outperformed‌ ‌the‌ ‌
standard‌ ‌feed‌ ‌forward‌ ‌neural‌ ‌network,‌ ‌there‌ ‌are‌ ‌a‌ ‌number‌ ‌of‌ ‌limitations‌ ‌to‌ ‌be‌ ‌
considered.‌ ‌First‌ ‌of‌ ‌all,‌ ‌the‌ ‌artificial‌ ‌implementation‌ ‌of‌ ‌each‌ ‌biological‌ ‌feature‌ ‌is‌ ‌a‌ ‌gross‌ ‌
simplification‌ ‌of‌ ‌their‌ ‌real‌ ‌biological‌ ‌counterparts.‌ ‌Although‌ ‌the‌ ‌proposed‌ ‌model‌ ‌has‌ ‌a‌ ‌
greater‌ ‌emphasis‌ ‌on‌ ‌neuroscience‌ ‌than‌ ‌modern‌ ‌networks,‌ ‌it‌ ‌is‌ ‌still‌ ‌far‌ ‌from‌ ‌a‌ ‌one-to-one‌ ‌
representation.‌ ‌Also,‌ ‌the‌ ‌field‌ ‌of‌ ‌neuroscience‌ ‌still‌ ‌needs‌ ‌further‌ ‌exploration‌ ‌before‌ ‌any‌ ‌
definite‌ ‌models‌ ‌of‌ ‌neural‌ ‌connectivity‌ ‌or‌ ‌plasticity‌ ‌are‌ ‌created,‌ ‌this‌ ‌is‌ ‌why‌ ‌teams‌ ‌like‌ ‌
Numenta‌ ‌are‌ ‌actively‌ ‌researching‌ ‌this‌ ‌very‌ ‌topic.‌ ‌ ‌
Another‌ ‌major‌ ‌limit‌ ‌on‌ ‌this‌ ‌experiment‌ ‌were‌ ‌the‌ ‌loading‌ ‌times‌ ‌for‌ ‌training.‌ ‌While‌ ‌
the‌ ‌control‌ ‌algorithm‌ ‌trained‌ ‌in‌ ‌seconds,‌ ‌the‌ ‌manipulated‌ ‌algorithm‌ ‌took‌ ‌over‌ ‌two‌ ‌hours.‌ ‌
This‌ ‌was‌ ‌a‌ ‌result‌ ‌of‌ ‌heavy‌ ‌computation‌ ‌when‌ ‌representing‌ ‌individual‌ ‌synapses‌ ‌and‌ ‌
neurotransmitters,‌ ‌the‌ ‌tradeoff‌ ‌being‌ ‌biological‌ ‌accuracy.‌ ‌Still,‌ ‌since‌ ‌the‌ ‌activity‌ ‌of‌ ‌a‌ ‌
31‌ ‌
neuron‌ ‌will‌ ‌affect‌ ‌the‌ ‌same‌ ‌R ‌values‌ ‌every‌ ‌time,‌ ‌receptors‌ ‌will‌ ‌change‌ ‌by‌ ‌the‌ ‌same‌ ‌
amount‌ ‌and‌ ‌not‌ ‌have‌ ‌a‌ ‌unique‌ ‌affect‌ ‌on‌ ‌each‌ ‌neurotransmitter‌ ‌output‌ ‌(Figure‌ ‌24).‌ ‌
A‌ ‌few‌ ‌other‌ ‌limitations‌ ‌to‌ ‌be‌ ‌considered‌ ‌are‌ ‌the‌ ‌size‌ ‌and‌ ‌simplicity‌ ‌of‌ ‌a‌ ‌dataset‌ ‌
with‌ ‌only‌ ‌256‌ ‌binary‌ ‌numbers‌ ‌(more‌ ‌difficult‌ ‌data‌ ‌may‌ ‌yield‌ ‌a‌ ‌different‌ ‌result),‌ ‌and‌ ‌that‌ ‌
the‌ ‌backpropagation‌ ‌algorithm‌ ‌(Figure‌ ‌18)‌ ‌only‌ ‌considers‌ ‌neurons‌ ‌and‌ ‌not‌ ‌the‌ ‌individual‌ ‌
synapses‌ ‌with‌ ‌unique‌ ‌receptor‌ ‌and‌ ‌neurotransmitter‌ ‌values.‌ ‌Respectively,‌ ‌this‌ ‌is‌ ‌why‌ ‌
the‌ ‌loss‌ ‌values‌ ‌were‌ ‌so‌ ‌low‌ ‌and‌ ‌why‌ ‌the‌ ‌proposed‌ ‌model‌ ‌was‌ ‌not‌ ‌entirely‌ ‌biologically‌ ‌
accurate.‌ ‌
Finally,‌ ‌the‌ ‌manipulated‌ ‌neural‌ ‌network‌ ‌competed‌ ‌against‌ ‌a‌ ‌standard‌ ‌feed‌ ‌
forward‌ ‌network‌ ‌without‌ ‌modern‌ ‌regularization‌ ‌methods‌ ‌such‌ ‌as‌ ‌dropout,‌ ‌or‌ ‌
normalization,‌ ‌which‌ ‌are‌ ‌common‌ ‌today‌ ‌and‌ ‌can‌ ‌increase‌ ‌accuracy‌ ‌(Brownlee,‌ ‌2016;‌ ‌
Keita‌ ‌Kurita,‌ ‌2018).‌ ‌It‌ ‌might‌ ‌not‌ ‌have‌ ‌outperformed‌ ‌a‌ ‌hyper-optimized‌ ‌network.‌ ‌
 ‌
Conclusions‌ ‌and‌ ‌Further‌ ‌Directions‌ ‌
In‌ ‌regards‌ ‌to‌ ‌the‌ ‌effect‌ ‌of‌ ‌principles‌ ‌of‌ ‌neural‌ ‌connectivity‌ ‌and‌ ‌neuroplasticity‌ ‌on‌ ‌
the‌ ‌recognition‌ ‌of‌ ‌binary‌ ‌patterns,‌ ‌the‌ ‌proposed‌ ‌model‌ ‌had‌ ‌less‌ ‌overall‌ ‌loss‌ ‌and‌ ‌
performed‌ ‌better‌ ‌in‌ ‌less‌ ‌training‌ ‌iterations‌ ‌than‌ ‌the‌ ‌controlled‌ ‌neural‌ ‌network.‌ ‌In‌ ‌terms‌ ‌
of‌ ‌accuracy,‌ ‌this‌ ‌would‌ ‌indicate‌ ‌increased‌ ‌accuracy‌ ‌of‌ ‌the‌ ‌manipulated‌ ‌model‌ ‌as‌ ‌well,‌ ‌
despite‌ ‌the‌ ‌inability‌ ‌to‌ ‌properly‌ ‌test‌ ‌it.‌ ‌
The‌ ‌most‌ ‌important‌ ‌takeaway‌ ‌from‌ ‌this‌ ‌experiment‌ ‌is‌ ‌the‌ ‌effectiveness‌ ‌of‌ ‌the‌ ‌
neuroscience-based‌ ‌model,‌ ‌since‌ ‌every‌ ‌biological‌ ‌equation‌ ‌was‌ ‌derived‌ ‌from‌ ‌research‌ ‌
instead‌ ‌of‌ ‌being‌ ‌used‌ ‌to‌ ‌directly‌ ‌enhance‌ ‌the‌ ‌feed‌ ‌forward‌ ‌neural‌ ‌network.‌ ‌In‌ ‌theory,‌ ‌the‌ ‌
32‌ ‌
novel‌ ‌method‌ ‌should‌ ‌have‌ ‌succeeded,‌ ‌and‌ ‌it‌ ‌did‌ ‌(all‌ ‌limitations‌ ‌considered).‌ ‌The‌ ‌next‌ ‌
steps‌ ‌would‌ ‌be‌ ‌to‌ ‌determine‌ ‌the‌ ‌accuracy‌ ‌of‌ ‌the‌ ‌manipulated‌ ‌model‌ ‌on‌ ‌non-binary‌ ‌data,‌ ‌
such‌ ‌as‌ ‌pictures‌ ‌or‌ ‌text.‌ ‌Also,‌ ‌it‌ ‌would‌ ‌be‌ ‌worth‌ ‌considering‌ ‌exploring‌ ‌neural‌ ‌topology‌ ‌--‌ ‌
three-dimensional,‌ ‌non-fully‌ ‌connected‌ ‌neural‌ ‌networks‌ ‌--‌ ‌and‌ ‌specialized‌ ‌receptors,‌ ‌
neurotransmitters,‌ ‌and‌ ‌neuronal‌ ‌cells‌ ‌(CITATION).‌ ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
33‌ ‌
References‌ ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
34‌ ‌
Appendix‌ ‌I‌ ‌
Controlled‌ ‌Neural‌ ‌Network‌ ‌
 ‌
35‌ ‌
36‌ ‌
 ‌
 ‌
37‌ ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
 ‌
38‌ ‌
Appendix‌ ‌II‌ ‌
Manipulated‌ ‌neural‌ ‌Network‌ ‌
 ‌
39‌ ‌
40‌ ‌
41‌ ‌
42‌ ‌
43‌ ‌
 ‌

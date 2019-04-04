# DisVoice

### Original (https://github.com/jcvasquezc/DisVoice) de J. C. Vasquez-Correa.
#### Cambios añadidos al original**:
 - **Comentar** líneas que utilizan **Kaldi** en estructura de Disvoice:
     - phonation.py lineas 71, 316, 330. Ejemplo: `#from kaldi_io import write_mat, write_vec_flt`
     - Más líneas en glotal.py y articulation.py
 - (*Windows*) En praat_functions.py, cuando construyye los comandos **cambiar `praat` por `..\\praat\\praat.exe`**. Esto es debido a que en windows prat es un ejecutable que se encuentra en la carpeta DisVoice/praat y nuestro script se ejecuta desde /Disvoice/phonation (y articulation o prosody)
 
------ 
DisVoice is a python framework designed to compute features from pathological speech. Disvoice computes phonation articulation, and prosody-based features both from sustained vowels and continuous speech utterances with the aim to evaluate the communication capabilities of patients with different voice disorders including diseases with functional origin such as larinx cancer or nodules; craneo-facial based disorders such as hipernasality developed by cleft-lip and palate; or neurodegenerative disorders such as Parkinson's disease.

For additional information please see phonation, articulaton, or prosody folders.


### Requeriments

- [Praat](http://www.fon.hum.uva.nl/praat/) - software for speech analysis.
- [Pysptk](http://pysptk.readthedocs.io/en/latest/) - python framework for speech analysis.

To install the requeriments, please run

```sh
install.sh
```

For Kaldi output Kaldi must be installed beforehand and the path at kaldi-io/kaldi-io.py:line 14:
"os.environ['KALDI_ROOT']='/mnt/matylda5/iveselyk/Tools/kaldi-trunk'"
should be changed to with path to the proper Kaldi root directory.


## Reference

If you use this code for research purpose, please cite one of the following articles

[[1]](http://www.sciencedirect.com/science/article/pii/S105120041730146X). J. R. Orozco-Arroyave, J. C. Vásquez-Correa et al. "NeuroSpeech: An open-source software for Parkinson's speech analysis." Digital Signal Processing (2017).

License
----

MIT

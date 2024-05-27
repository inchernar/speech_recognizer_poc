```bash
pip3 install vosk
curl -o ./model.zip https://alphacephei.com/vosk/models/vosk-model-ru-0.22.zip
unzip model.zip
mv vosk-model-ru-0.22/ model
rm -rf model.zip
python app.py
```

```
LOG (VoskAPI:ReadDataFiles():model.cc:213) Decoding params beam=13 max-active=7000 lattice-beam=6
LOG (VoskAPI:ReadDataFiles():model.cc:216) Silence phones 1:2:3:4:5:6:7:8:9:10
LOG (VoskAPI:RemoveOrphanNodes():nnet-nnet.cc:948) Removed 1 orphan nodes.
LOG (VoskAPI:RemoveOrphanComponents():nnet-nnet.cc:847) Removing 2 orphan components.
LOG (VoskAPI:Collapse():nnet-utils.cc:1488) Added 1 components, removed 2
LOG (VoskAPI:ReadDataFiles():model.cc:248) Loading i-vector extractor from model/ivector/final.ie
LOG (VoskAPI:ComputeDerivedVars():ivector-extractor.cc:183) Computing derived variables for iVector extractor
LOG (VoskAPI:ComputeDerivedVars():ivector-extractor.cc:204) Done.
LOG (VoskAPI:ReadDataFiles():model.cc:279) Loading HCLG from model/graph/HCLG.fst
LOG (VoskAPI:ReadDataFiles():model.cc:297) Loading words from model/graph/words.txt
LOG (VoskAPI:ReadDataFiles():model.cc:308) Loading winfo model/graph/phones/word_boundary.int
LOG (VoskAPI:ReadDataFiles():model.cc:315) Loading subtract G.fst model from model/rescore/G.fst
LOG (VoskAPI:ReadDataFiles():model.cc:317) Loading CARPA model from model/rescore/G.carpa
LOG (VoskAPI:ReadDataFiles():model.cc:323) Loading RNNLM model from model/rnnlm/final.raw
{
  "text" : "так провожу проверку звука для расшифровки текста текст на русском языке раз-два раз-два проверяем"
}
```

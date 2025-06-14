###  Dependencies

Install required packages:

pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
pip install transformers accelerate
pip install scispacy==0.5.1
pip install https://s3-us-west-2.amazonaws.com/ai2-s2-scispacy/releases/en_ner_bc5cdr_md-0.5.1.tar.gz

Models Used

- **Local LLM**: [`unsloth/DeepSeek-R1-Distill-Qwen-7B`](https://huggingface.co/unsloth/DeepSeek-R1-Distill-Qwen-7B)
  - Loaded via `transformers`, quantized using `bnb-4bit`
- **spaCy NER**: `en_ner_bc5cdr_md` `en_core_web_sm`from SciSpaCy for medical-specific entity labeling


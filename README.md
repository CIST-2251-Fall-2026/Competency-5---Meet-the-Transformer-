# Competency 5 - Meet the Transformer
# Overview
I used DistilGPT2 to test how AI generates text and how different settings affect the results.
## Model Information
* Model: distilbert/distilgpt2
* PyTorch: 2.15.0+cpu
* Transformers: 5.22.1
* License: Apache 2.0
# Setup
Install Python and run:
`python -m pip install torch transformers`
Open the notebook in VS Code and run each cell.
# What I Learned
**Training vs. Inference:** Training teaches AI patterns, while inference uses those patterns to generate text.
**Tokens:** Tokens are pieces of text. Some words are split into multiple tokens.
**Context:** Changing a prompt can change the response, but the model does not always follow instructions.
**Temperature:** Lower temperatures usually give more predictable responses. Higher temperatures can make responses more random.
# Experiment Results
I tested the same prompt with seeds 10, 20, and 30. Each seed produced a different response.
I also tested temperatures 0.3, 0.7, and 1.2 using seed 42. The lower temperature was more predictable, while the higher temperature produced less reliable text.
When I changed the prompt to explain AI to different audiences, the responses changed, but the model did not explain things appropriately.
# Model Limitations
When I tested "The capital of France is", the model did not answer Paris. Instead, it talked about military and economic security.
This could be a problem for customers because they might receive confusing or incorrect information.
# Conclusion
I learned how transformers generate text and how settings affect their responses. DistilGPT2 is useful for experimenting, but more testing would be needed before using it in a real product.
##References
Hugging Face. DistilGPT2.
https://huggingface.co/distilbert/distilgpt2
Géron, A. (2025). Hands-On Machine Learning with Scikit-Learn and PyTorch. O'Reilly Media.
Grootendorst, M., & Alammar, J. (2026). An Illustrated Guide to AI Agents. O'Reilly Media.
I tried a lot of models, including BILP, GPT, CLIP, CLVP, but they all reported errors during operation. It took me a lot of time. Finally, I chose the git model, My optimizer is set to Optimizer = optim.SGD(model.parameters(), lr=0.005, momentum=0.9, weight_decay=1e-6, dampening=0, nesterov=True).

I also changed the database loading method to inputs = self.processor(images=img, text=caption, padding="max_length", return_tensors="pt"), attention_mask was added to encoding.

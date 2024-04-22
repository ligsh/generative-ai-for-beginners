# Introduction to Generative AI and Large Language Models

[![Introduction to Generative AI and Large Language Models](./images/01-lesson-banner.png?WT.mc_id=academic-105485-koreyst)](https://learn.microsoft.com/_themes/docs.theme/master/en-us/_themes/global/video-embed.html?id=36c6795a-e63c-46dd-8d69-df8bbe6e7bc9?WT.mc_id=academic-105485-koreyst)

*(Click the image above to view video of this lesson)*

Generative AI is artificial intelligence capable of generating text, images and other types of content(生成式AI是AI生成文本、图像及其他类型内容的能力). What makes it a fantastic technology is that it democratizes AI, anyone can use it with as little as a text prompt, a sentence written in a natural language. There's no need for you to learn a language like Java or SQL to accomplish something worthwhile, all you need is to use your language, state what you want and out comes a suggestion from an AI model. The applications and impact for this is huge, you write or understand reports, write applications and much more, all in seconds. 

In this curriculum, we’ll explore how our startup leverages generative AI to unlock new scenarios in the education world and how we address the inevitable challenges associated with the social implications of its application and the technology limitations.

## Introduction

This lesson will cover:

* Introduction to the business scenario: our startup idea and mission.
* Generative AI and how we landed on the current technology landscape.
* Inner working of a large language model.
* Main capabilities and practical use cases of Large Language Models.

## Learning Goals

After completing this lesson, you will understand:

* What generative AI is and how Large Language Models work（生成式AI是什么以及大语言模型是如何工作的）.
* How you can leverage large language models for different use cases, with a focus on education scenarios.

## Scenario: our educational startup 

Generative Artificial Intelligence (AI) represents the pinnacle of AI technology, pushing the boundaries of what was once thought impossible. Generative AI models have several capabilities and applications, but for this curriculum we'll explore how it's revolutionizing education through a fictional startup. We'll refer to this startup as *our startup*. Our startup works in the education domain with the ambitious mission statement of 

> *improving accessibility in learning, on a global scale, ensuring equitable access to education and providing personalized learning experiences to every learner, according to their needs*.

Our startup team is aware we’ll not be able to achieve this goal without leveraging one of the most powerful tools of modern times – Large Language Models (LLMs).

Generative AI is expected to revolutionize the way we learn and teach today, with students having at their disposal virtual teachers 24 hours a day who provide vast amounts of information and examples, and teachers able to leverage innovative tools to assess their students and give feedback.

![Five young students looking at a monitor - image by DALLE2](./images/students-by-DALLE2.png?WT.mc_id=academic-105485-koreyst)

To start, let’s define some basic concepts and terminology we’ll be using throughout the curriculum.

## How did we get Generative AI?

Despite the extraordinary *hype* created lately by the announcement of generative AI models, this technology is decades in the making, with the first research efforts dating back to 60s. We're now at a point with AI having human cognitive capabilities, like conversation as shown by for example [OpenAI ChatGPT](https://openai.com/chatgpt) or [Bing Chat](https://www.microsoft.com/edge/features/bing-chat?WT.mc_id=academic-105485-koreyst), which also uses a GPT model for the web search Bing conversations.

Backing up a bit, the  very first prototypes of AI consisted of typewritten(打印的) chatbots（打印的聊天机器人？能够以打印方式输出内容的聊天机器人）, relying on a knowledge base extracted from a group of experts and represented into a computer. The answers in the knowledge base were triggered by keywords appearing in the input text.
However, it soon became clear that such approach, using typewritten chatbots, did not scale well.
最早的AI原型是一个打印的聊天机器人，它依赖于一个知识库。输入文本中的关键词触发知识库中的答案。很快，使用打印的聊天机器人的扩展并不好。

### A statistical approach to AI: Machine Learning (以统计的形式达成AI：机器学习)

A turning point arrived during the 90s, with the application of a statistical approach to text analysis(转折点出现在上世纪90年代，即出现了以统计方法对文件进行分析的方式). This led to the development of new algorithms – known with the name of machine learning - able to learn patterns from data, without being explicitly programmed(这导致了新算法——成为机器学习的开发，这种算法从数据中学到“模式‘，而不需要显示的通过编程方式得到). This approach allows a machine to simulate human language understanding(这种方法允许机器模拟人类语言的理解方式): a statistical model is trained on text-label pairings, enabling the model to classify unknown input text with a pre-defined label representing the intention of the message(在文本-标签对上训练一个统计模型，使得该模型能够对 带有预定义标签的未知输入文本进行分类).

### Neural networks and modern virtual assistants (神经网络和现代虚拟助手)

In more recent times, the technological evolution of the hardware, capable of handling larger amounts of data and more complex computations, encouraged research in the AI fields, leading to the development of advanced machine learning algorithms – called neural networks or deep learning algorithms(近来，随着硬件技术的进步，能够处理更大量的数据以及进行更为复杂的计算，存进了AI领域的研究，导致了更为高级的机器学习算法——称为神经网络或者深度学习算法).

Neural networks (and in particular Recurrent Neural Networks – RNNs) significantly enhanced natural language processing, enabling the representation of the meaning of text in a more meaningful way, valuing the context of a word in a sentence（神经网络显著增强了自然语言的处理，使文本的意义以一种更为有意义的方式呈现，即在一个橘句子的上下文内评估一个单词的含义）.

This is the technology that powered the virtual assistants born in the first decade of the new century, very proficient in interpreting the human language, identifying a need, and performing an action to satisfy it – like answering with a pre-defined script or consuming a 3rd party service.

### Present day, Generative AI (当前，生成式AI)

So that’s how we came to Generative AI today, which can be seen as a subset of deep learning(生成式AI可以认为是深度学习的一个子集).

![AI, ML, DL and Generative AI](./images/AI-diagram.png?WT.mc_id=academic-105485-koreyst)

After decades of research in the AI field, a new model architecture – called *Transformer* – overcame the limits of RNNs, being able to get much longer sequences of text as input(在AI领域数十年的研究，一个新的模型结构——称为Transformer——突破了RNN的限制，能够得到更长的文本序列作为输入). Transformers are based on the attention mechanism, enabling the model to give different weights to the inputs it receives, ‘paying more attention’ where the most relevant information is concentrated, regardless of their order in the text sequence(Transformers基于注意力机制，使模型能够对它接受的输入给予不同的权重，即对最相关的信息给予更多的注意力，而不管他们在文本序列中的顺序).

Most of the recent generative AI models – also known as Large Language Models (LLMs), since they work with textual inputs and outputs – are indeed based on this architecture（大多数最新的生成式AI模型——也被叫做大语言模型，因为它们和文本性的输入输出一起工作——就是居于这种结构。 什么是Model？第一次出现是作为一种“统计模型”）. What’s interesting about these models – trained on a huge amount of unlabeled data from diverse(不同的) sources like books, articles and websites – is that they can be adapted to a wide variety of tasks and generate grammatically correct text with a semblance of creativity. So, not only did they incredibly enhance the capacity of a machine to ‘understand’ an input text, but they enabled their capacity to generate an original response in human language(关于这些模型，最有趣的是).

## How do large language models work?

In the next chapter we are going to explore different types of Generative AI models, but for now let’s have a look at how large language models work, with a focus on OpenAI GPT (Generative Pre-trained Transformer) models.

* **Tokenizer, text to numbers**（tokenizer，从文本到数字）: Large Language Models receive a text as input and generate a text as output(LLM接受文本作为输入，生成文本作为输出). However, being statistical models, they work much better with numbers than text sequences. That’s why every input to the model is processed by a tokenizer, before being used by the core model(在被核心模型处理之前，每个输入都需要被tokenizer进行处理). A token is a chunk of text – consisting of a variable number of characters, so the tokenizer's main task is splitting the input into an array of tokens. Then, each token is mapped with a token index, which is the integer encoding of the original text chunk(然后，每个token映射到token index，token index是原始文本块的整数编码).

![Example of tokenization](./images/tokenizer-example.png?WT.mc_id=academic-105485-koreyst)

* **Predicting output tokens(预测输出tokens）**: Given n tokens as input (with max n varying from one model to another)(给定n个token作为input，不同的model能够接受的n的最大值不同), the model is able to predict one token as output(model可以预测一个token作为输出). This token is then incorporated into the input of the next iteration, in an expanding window pattern, enabling a better user experience of getting one (or multiple) sentence as an answer(这个token然后又被组合到input中，由model在根据新的input预测下一个token，如此循环往复). This explains why, if you ever played with ChatGPT, you might have noticed that sometimes it looks like it stops in the middle of a sentence.

* **Selection process, probability distribution**: The output token is chosen by the model according to its probability of occurring after the current text sequence(被模型所选择的输出token是基于其在当前文本序列之后发生的可能性). This is because the model predicts a probability distribution over all possible ‘next tokens’, calculated based on its training. However, not always the token with the highest probability is chosen from the resulting distribution(具有最高可能性的token并不总是被选中作为输出). A degree of randomness is added to this choice(在选择下一个token的过程中，加入了一定程度的随机性), in a way that the model acts in a non-deterministic fashion - we do not get the exact same output for the same input. This degree of randomness is added to simulate the process of creative thinking and it can be tuned using a model parameter called temperature(加入这种随机性来模拟创造性思维，这种随机性可以使用被称为“温度”的模型参数进行调整).

## How can our startup leverage Large Language Models?(我们该怎言开始借助LLM？)

Now that we have a better understanding of the inner working of a large language model, let’s see some practical examples of the most common tasks they can perform pretty well, with an eye to our business scenario(现在我们已经对LLM的内部工作有了更好的理解，让我们看一些它们完成很好的最常见任务的例子).
We said that the main capability of a Large Language Model is *generating a text from scratch, starting from a textual input, written in natural language*(我们已经说过，LLM的主要能力是：以自然语言书写的文本作为输入，从0开始生成文本).

But what kind of textual input and output?(那么是什么类型的文本输入和输出呢？)
The input of a large language model is known as prompt(大语言模型的输入被称为prompt), while the output is known as completion(而其输出称为completion), term that refers to the model mechanism of generating the next token to complete the current input(这个属于来自于模型生成下一个token来“完成”当前输入的机制). We are going to dive deep into what is a prompt and how to design it in a way to get the most out of our model(我们将深入了解什么是prompt，以及如何来设计prompt). But for now, let’s just say that a prompt may include(现在，我们可以认为prompt包括):

* An **instruction** specifying the type of output we expect from the model. This instruction sometimes might embed some examples or some additional data(一个指令，指定我们期望从模型中获得输出的类型。这个指令有时会包含一些示例或一些条件数据).

    1. Summarization of an article, book, product reviews and more, along with extraction of insights from unstructured data.
    
    ![Example of summarization](./images/summarization-example.png?WT.mc_id=academic-105485-koreyst)

    <br>
    
    2. Creative ideation and design of an article, an essay, an assignment or more.
    
    ![Example of creative writing](./images/creative-writing-example.png?WT.mc_id=academic-105485-koreyst)

    <br>
    
* A **question**, asked in the form of a conversation with an agent(一个问题，以和一个代理谈话的形式问出).
  
![Example of conversation](./images/conversation-example.png?WT.mc_id=academic-105485-koreyst)

<br>

* A chunk of **text to complete**, which implicitly is an ask for writing assistance(一段未完成的文本，这是个隐式的请求).
   
![Example of text completion](./images/text-completion-example.png?WT.mc_id=academic-105485-koreyst)

<br>

* A chunk of **code** together with the ask of explaining and documenting it, or a comment asking to generate a piece of code performing a specific task（要求对一段程序代码进行解释或文档说明，或者是针对一个“注释”要求生成一段代码来执行特定任务）.

![Coding example](./images/coding-example.png?WT.mc_id=academic-105485-koreyst)

<br>

The examples above are quite simple and don’t want to be an exhaustive demonstration of Large Language Models capabilities. They just want to show the potential of using generative AI, in particular but not limited to educational context.

Also, the output of a generative AI model is not perfect and sometimes the creativity of the model can work against it, resulting in an output which is a combination of words that the human user can interpret as a mystification of reality, or it can be offensive(同时，生成式AI model的输出并不完美，有时模型的创造性导致的输出，人类会迷惑不解或感到具有冒犯性). Generative AI is not intelligent - at least in the more comprehensive definition of intelligence, including critical and creative reasoning or emotional intelligence; it is not deterministic, and it is not trustworthy, since fabrications, such as erroneous references, content, and statements, may be combined with correct information, and presented in a persuasive and confident manner. In the following lessons, we’ll be dealing with all these limitations and we’ll see what we can do to mitigate them.

## Assignment 作业

Your assignment is to read up more on [generative AI](https://en.wikipedia.org/wiki/Generative_artificial_intelligence?WT.mc_id=academic-105485-koreyst) and try to identify an area where you would add generative AI today that doesn't have it. How would the impact be different from doing it the "old way", can you do something you couldn't before, or are you faster? Write a 300 word summary on what your dream AI startup would look like and include headers like "Problem", "How I would use AI", "Impact" and optionally a business plan. 

If you did this task, you might even be ready to apply to Microsoft's incubator, [Microsoft for Startups Founders Hub](https://www.microsoft.com/startups?WT.mc_id=academic-105485-koreyst) we offer credits for both Azure, OpenAI, mentoring and much more, check it out!

## Knowledge check

What's true about large language models?

1. You get the exact same response every time.
1. It does things perfectly, great at adding numbers, produce working code etc.
1. The response may vary despite using the same prompt. It's also great at giving you a first draft of something, be it text or code. But you need to improve on the results.

A: 3, an LLM is non-deterministic, the response vary, however, you can control its variance via a temperature setting. You also shouldn't expect it to do things perfectly, it's here to do the heavy-lifting for you which often means you get a good first attempt at something that you need to gradually improve.

## Great Work! Continue the Journey 

After completing this lesson, check out our [Generative AI Learning collection](https://aka.ms/genai-collection?WT.mc_id=academic-105485-koreyst) to continue leveling up your Generative AI knowledge!

Head over to Lesson 2 where we will look at how to [explore and compare different LLM types](../02-exploring-and-comparing-different-llms/README.md?WT.mc_id=academic-105485-koreyst)!

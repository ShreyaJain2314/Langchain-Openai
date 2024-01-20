# Langchain-Openai
Chatbots are one of the central LLM use-cases. The core features of chatbots are that they can have long-running conversations and have access to information that users want to know about.

Aside from basic prompting and LLMs, memory and retrieval are the core components of a chatbot. Memory allows a chatbot to remember past interactions, and retrieval provides a chatbot with up-to-date, domain-specific information.

#Overview
The chat model interface is based around messages rather than raw text. Several components are important to consider for chat:

chat model: See here for a list of chat model integrations and here for documentation on the chat model interface in LangChain. You can use LLMs (see here) for chatbots as well, but chat models have a more conversational tone and natively support a message interface.
prompt template: Prompt templates make it easy to assemble prompts that combine default messages, user input, chat history, and (optionally) additional retrieved context.
memory: See here for in-depth documentation on memory types
retriever (optional): See here for in-depth documentation on retrieval systems. These are useful if you want to build a chatbot with domain-specific knowledge.

#Memory
As we mentioned above, the core component of chatbots is the memory system. One of the simplest and most commonly used forms of memory is ConversationBufferMemory:

This memory allows for storing of messages in a buffer
When called in a chain, it returns all of the messages it has stored
LangChain comes with many other types of memory, too. See here for in-depth documentation on memory types.

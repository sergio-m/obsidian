{
  "id": "sCy7Dz1t2CXusiPB",
  "meta": {
    "instanceId": "2cdd9c593c5820bad56f93ddf9a9bb70d8c9e27fcdca4b21793502db1aae1d9d",
    "templateCredsSetupCompleted": true
  },
  "name": "Prompt generator",
  "tags": [],
  "nodes": [
    {
      "id": "4196a5c9-1217-4216-a3dc-ca752fc7e728",
      "name": "On form submission",
      "type": "n8n-nodes-base.formTrigger",
      "position": [
        -1140,
        -20
      ],
      "webhookId": "d4dc2007-3c6d-4a26-b1f0-b5fbe6c8319c",
      "parameters": {
        "options": {
          "customCss": "/* N8N Landing Page CSS - Correct Selectors Based on HTML */\n\n/* Style the main form card */\n.card {\n\tposition: relative;\n\tmax-width: 500px;\n\tmargin: 20px auto;\n\tpadding: 20px;\n\tbackground: white !important;\n\tborder-radius: 12px;\n\tbox-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);\n\tfont-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;\n}\n\n/* Add custom header with gradient */\n.card:before {\n\tcontent: '';\n\tdisplay: block;\n\theight: 50px;\n\tbackground: linear-gradient(135deg, #6366f1 0%, #8b5cf6 100%);\n\tposition: relative;\n\tmargin: -20px -20px 30px -20px;\n\tborder-radius: 12px 12px 0 0;\n}\n\n/* Style the form header */\n.form-header {\n\ttext-align: center !important;\n\tcolor: #1f2937 !important;\n\tfont-weight: 700 !important;\n\tmargin: 80px 0 15px 0 !important;\n\tfont-size: 2.2em !important;\n\tposition: relative;\n\tz-index: 5;\n}\n\n/* Style any h1, h2 elements in the form */\n.card h1,\n.card h2 {\n\ttext-align: center !important;\n\tcolor: #1f2937 !important;\n\tfont-weight: 700 !important;\n\tmargin: 80px 0 15px 0 !important;\n\tfont-size: 2.2em !important;\n\tposition: relative;\n\tz-index: 5;\n}\n\n/* Style paragraphs and description text */\n.card p {\n\ttext-align: center !important;\n\tcolor: #6b7280 !important;\n\tfont-size: 1.1em !important;\n\tmargin-bottom: 30px !important;\n\tline-height: 1.5 !important;\n\tposition: relative;\n\tz-index: 5;\n}\n\n/* Style the inputs wrapper */\n.inputs-wrapper {\n\tposition: relative;\n\tz-index: 5;\n}\n\n/* Style all input fields */\n.card input[type=\"text\"],\n.card input[type=\"email\"],\n.card input[type=\"tel\"],\n.card input[type=\"number\"],\n.card textarea,\n.card select {\n\twidth: 100% !important;\n\tpadding: 12px 16px !important;\n\tborder: 2px solid #e5e7eb !important;\n\tborder-radius: 8px !important;\n\tfont-size: 16px !important;\n\ttransition: border-color 0.3s ease !important;\n\tmargin-bottom: 15px !important;\n\tbox-sizing: border-box !important;\n}\n\n.card input[type=\"text\"]:focus,\n.card input[type=\"email\"]:focus,\n.card input[type=\"tel\"]:focus,\n.card input[type=\"number\"]:focus,\n.card textarea:focus,\n.card select:focus {\n\toutline: none !important;\n\tborder-color: #6366f1 !important;\n\tbox-shadow: 0 0 0 3px rgba(99, 102, 241, 0.1) !important;\n}\n\n/* Style the submit button */\n.card button[type=\"submit\"],\n.card input[type=\"submit\"] {\n\tbackground: linear-gradient(135deg, #ff6b6b 0%, #ff8e8e 100%) !important;\n\tcolor: white !important;\n\tborder: none !important;\n\tpadding: 15px 40px !important;\n\tborder-radius: 10px !important;\n\tfont-size: 18px !important;\n\tfont-weight: 600 !important;\n\tcursor: pointer !important;\n\twidth: 100% !important;\n\tmargin-top: 20px !important;\n\ttransition: all 0.3s ease !important;\n\tbox-shadow: 0 4px 15px rgba(255, 107, 107, 0.3) !important;\n\tposition: relative;\n\tz-index: 5;\n}\n\n.card button[type=\"submit\"]:hover,\n.card input[type=\"submit\"]:hover {\n\ttransform: translateY(-2px) !important;\n\tbox-shadow: 0 6px 20px rgba(255, 107, 107, 0.4) !important;\n}\n\n/* Style the body to complement the form */\nbody.vsc-initialized {\n\tbackground: #f8fafc !important;\n\tfont-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif !important;\n\tmargin: 0 !important;\n\tpadding: 20px !important;\n}\n\n/* Style the container div */\n.container {\n\tmax-width: 600px !important;\n\tmargin: 0 auto !important;\n}\n\n/* Mobile responsive */\n@media (max-width: 768px) {\n\t.card {\n\t\tmargin: 10px !important;\n\t\tpadding: 15px !important;\n\t}\n\t\n\t.card:before {\n\t\theight: 50px !important;\n\t\tmargin: -15px -15px 20px -15px !important;\n\t}\n\t\n\t.card:after {\n\t\ttop: 35px !important;\n\t\tfont-size: 35px !important;\n\t}\n\t\n\t.form-header,\n\t.card h1,\n\t.card h2 {\n\t\tfont-size: 1.8em !important;\n\t\tmargin: 60px 0 15px 0 !important;\n\t}\n}",
          "buttonLabel": "Let's Generate",
          "appendAttribution": false
        },
        "formTitle": "🚀 AI Prompt Generator",
        "formDescription": "Create powerful prompts for your AI tools"
      },
      "typeVersion": 2.2
    },
    {
      "id": "bb9f2e02-a01e-4508-8ef0-37a9b9edd1ba",
      "name": "Google Gemini Chat Model",
      "type": "@n8n/n8n-nodes-langchain.lmChatGoogleGemini",
      "position": [
        -680,
        180
      ],
      "parameters": {
        "options": {},
        "modelName": "models/gemini-2.0-flash"
      },
      "credentials": {
        "googlePalmApi": {
          "id": "9BZpt0x33yMhJWqO",
          "name": "Google Gemini(PaLM) Api account 2"
        }
      },
      "typeVersion": 1
    },
    {
      "id": "1fa60776-44ca-4478-b3bd-28b6c8fb8355",
      "name": "Structured Output Parser",
      "type": "@n8n/n8n-nodes-langchain.outputParserStructured",
      "position": [
        -520,
        180
      ],
      "parameters": {
        "jsonSchemaExample": "[\n  {\n    \"fieldLabel\": \"Label for the question to ask\",\n    \"placeholder\": \"Short hint to guide the user’s answer\",\n    \"requiredField\": true,\n    \"fieldType\": \"text\"\n  }\n]"
      },
      "typeVersion": 1.2
    },
    {
      "id": "2ad0f046-36ff-4864-af2e-339763109a9c",
      "name": "BaseQuestions",
      "type": "n8n-nodes-base.form",
      "position": [
        -920,
        -20
      ],
      "webhookId": "cdf6ec24-43fe-4a6b-908a-9d17d3e0feec",
      "parameters": {
        "options": {
          "customCss": "/* Apply to all n8n form pages */\n.card {\n\tposition: relative;\n\tmax-width: 500px;\n\tmargin: 20px auto;\n\tpadding: 20px;\n\tbackground: white !important;\n\tborder-radius: 12px;\n\tbox-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);\n\tfont-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;\n}\n\n.card:before {\n\tcontent: '';\n\tdisplay: block;\n\theight: 50px;\n\tbackground: linear-gradient(135deg, #6366f1 0%, #8b5cf6 100%);\n\tposition: relative;\n\tmargin: -20px -20px 30px -20px;\n\tborder-radius: 12px 12px 0 0;\n}\n\n.card h1, .card h2 {\n\ttext-align: center !important;\n\tcolor: #1f2937 !important;\n\tfont-weight: 700 !important;\n\tmargin: 15px 0 !important;\n\tfont-size: 2em !important;\n}\n\n.card p {\n\tfont-size: 1.1em !important;\n\tline-height: 1.5 !important;\n}\n\n.inputs-wrapper {\n\tposition: relative;\n}\n\n.form-group {\n  margin-bottom: 15px;\n}\n\n.card input, .card textarea, .card select {\n\twidth: 100% !important;\n\tpadding: 12px 16px !important;\n\tborder: 2px solid #e5e7eb !important;\n\tborder-radius: 8px !important;\n\tfont-size: 16px !important;\n\tbox-sizing: border-box !important;\n\ttransition: border-color 0.3s ease !important;\n}\n\n.card input:focus, .card textarea:focus, .card select:focus {\n\tborder-color: #6366f1 !important;\n\tbox-shadow: 0 0 0 3px rgba(99, 102, 241, 0.1) !important;\n\toutline: none !important;\n}\n\n.card button[type=\"submit\"] {\n\tbackground: linear-gradient(135deg, #16a34a 0%, #22c55e 100%) !important;\n\tcolor: white !important;\n\tpadding: 15px 40px !important;\n\tborder-radius: 10px !important;\n\tfont-size: 18px !important;\n\tfont-weight: 600 !important;\n\tcursor: pointer !important;\n\twidth: 100% !important;\n\tbox-shadow: 0 4px 15px rgba(34, 197, 94, 0.3) !important;\n\ttransition: all 0.3s ease !important;\n}\n\n.card button[type=\"submit\"]:hover {\n\ttransform: translateY(-2px) !important;\n\tbox-shadow: 0 6px 20px rgba(34, 197, 94, 0.4) !important;\n}\n\n.error-hidden {\n    display: block;\n    position: relative;\n    color: var(--color-error);\n    text-align: left;\n    font-size: var(--font-size-error);\n    font-weight: 400;\n    visibility: hidden;\n    padding-top: 0;\n    padding-bottom: 0;\n}\n\n@media (max-width: 768px) {\n\t.card {\n\t\tmargin: 10px !important;\n\t\tpadding: 15px !important;\n\t}\n\t.card h1, .card h2 {\n\t\tfont-size: 1.6em !important;\n\t}\n  .card:before {\n    margin: -20px -15px 30px -15px;\n  }\n}\n",
          "formTitle": "Enrich Prompt",
          "buttonLabel": "Answer"
        },
        "formFields": {
          "values": [
            {
              "fieldType": "textarea",
              "fieldLabel": "What do you want to build ?",
              "placeholder": "i.e.  A B2B proposal generator for content marketing agency",
              "requiredField": true
            },
            {
              "fieldType": "textarea",
              "fieldLabel": "Tools I can access (N/A if no tools)",
              "placeholder": "i.e. Web Search, Email Threads, Google Sheets",
              "requiredField": true
            },
            {
              "fieldType": "textarea",
              "fieldLabel": "What Input can be expected ?",
              "placeholder": "i.e. The customer data like name, company, problems you can solve.",
              "requiredField": true
            },
            {
              "fieldType": "textarea",
              "fieldLabel": "What output do you expect ?",
              "placeholder": "i.e. A proposal for the company that is specific to the customer",
              "requiredField": true
            }
          ]
        }
      },
      "typeVersion": 1
    },
    {
      "id": "f7e1522a-3951-47fb-9e5a-5730ff3cf055",
      "name": "LoopQuestions",
      "type": "n8n-nodes-base.splitInBatches",
      "position": [
        0,
        60
      ],
      "parameters": {
        "options": {}
      },
      "executeOnce": false,
      "typeVersion": 3
    },
    {
      "id": "e2b5d3c4-cb4c-4f90-93a1-10784bd8a38e",
      "name": "RelevantQuestions",
      "type": "n8n-nodes-base.form",
      "position": [
        260,
        80
      ],
      "webhookId": "8d220b4e-1c9c-4f52-8d1f-0e5f396f7745",
      "parameters": {
        "options": {
          "customCss": "/* Apply to all n8n form pages */\n.card {\n\tposition: relative;\n\tmax-width: 500px;\n\tmargin: 20px auto;\n\tpadding: 20px;\n\tbackground: white !important;\n\tborder-radius: 12px;\n\tbox-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);\n\tfont-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;\n}\n\n.card:before {\n\tcontent: '';\n\tdisplay: block;\n\theight: 50px;\n\tbackground: linear-gradient(135deg, #6366f1 0%, #8b5cf6 100%);\n\tposition: relative;\n\tmargin: -20px -20px 30px -20px;\n\tborder-radius: 12px 12px 0 0;\n}\n\n.card h1, .card h2 {\n\ttext-align: center !important;\n\tcolor: #1f2937 !important;\n\tfont-weight: 700 !important;\n\tmargin: 15px 0 !important;\n\tfont-size: 2em !important;\n}\n\n.card p {\n\tfont-size: 1.1em !important;\n\tline-height: 1.5 !important;\n}\n\n.inputs-wrapper {\n\tposition: relative;\n}\n\n.form-group {\n  margin-bottom: 15px;\n}\n\n.card input, .card textarea, .card select {\n\twidth: 100% !important;\n\tpadding: 12px 16px !important;\n\tborder: 2px solid #e5e7eb !important;\n\tborder-radius: 8px !important;\n\tfont-size: 16px !important;\n\tbox-sizing: border-box !important;\n\ttransition: border-color 0.3s ease !important;\n}\n\n.card input:focus, .card textarea:focus, .card select:focus {\n\tborder-color: #6366f1 !important;\n\tbox-shadow: 0 0 0 3px rgba(99, 102, 241, 0.1) !important;\n\toutline: none !important;\n}\n\n.card button[type=\"submit\"] {\n\tbackground: linear-gradient(135deg, #16a34a 0%, #22c55e 100%) !important;\n\tcolor: white !important;\n\tpadding: 15px 40px !important;\n\tborder-radius: 10px !important;\n\tfont-size: 18px !important;\n\tfont-weight: 600 !important;\n\tcursor: pointer !important;\n\twidth: 100% !important;\n\tbox-shadow: 0 4px 15px rgba(34, 197, 94, 0.3) !important;\n\ttransition: all 0.3s ease !important;\n}\n\n.card button[type=\"submit\"]:hover {\n\ttransform: translateY(-2px) !important;\n\tbox-shadow: 0 6px 20px rgba(34, 197, 94, 0.4) !important;\n}\n\n.error-hidden {\n    display: block;\n    position: relative;\n    color: var(--color-error);\n    text-align: left;\n    font-size: var(--font-size-error);\n    font-weight: 400;\n    visibility: hidden;\n    padding-top: 0;\n    padding-bottom: 0;\n}\n\n@media (max-width: 768px) {\n\t.card {\n\t\tmargin: 10px !important;\n\t\tpadding: 15px !important;\n\t}\n\t.card h1, .card h2 {\n\t\tfont-size: 1.6em !important;\n\t}\n  .card:before {\n    margin: -20px -15px 30px -15px;\n  }\n}\n",
          "formTitle": "Questions to understand",
          "buttonLabel": "Answer"
        },
        "defineForm": "json",
        "jsonOutput": "=[{{ $('LoopQuestions').item.json }}]"
      },
      "typeVersion": 1
    },
    {
      "id": "1618be1e-222c-45d5-a85e-d76878971f60",
      "name": "MergeUserIntent",
      "type": "n8n-nodes-base.merge",
      "position": [
        500,
        -20
      ],
      "parameters": {},
      "typeVersion": 3.1
    },
    {
      "id": "cbd1fbb5-a530-4695-9f7a-d3c1fe394bb9",
      "name": "PromptGenerator",
      "type": "@n8n/n8n-nodes-langchain.chainLlm",
      "position": [
        740,
        -20
      ],
      "parameters": {
        "text": "={{ $('MergeUserIntent').item.json }}",
        "messages": {
          "messageValues": [
            {
              "message": "<role>\nYou are an expert AI prompt generator designed to turn semi-structured user inputs into effective and well-formatted prompts for downstream AI agents. Your goal is to craft high-quality prompts that follow strict formatting and enable the target AI agent to perform its task optimally. And to do that you'll be receiving the user's input like what they want to build, which tool AI can use, what input the ai need to expect and what output the user want from their ai agent. Also you'll be receiving some specific constraints for the ai agent to be taken care along with some clarifying questions.\n</role>\n\n<inputs>\nYou will receive a JSON array that includes:\n- The user's primary intent (e.g., what they want to build)\n- What tools they plan to use (or \"N/A\")\n- What input the tool will receive\n- What output they expect\n- Any constraints (e.g., token limits, length)\n- Up to 3 additional form answers for clarifying context (e.g., tone, style, audience)\n\nExample input:\n[\n  {\n    \"What do you want to build ?\": \"Video to LinkedIn post\",\n    \"Tools I can access (N/A if no tools)\": \"N/A\",\n    \"What Input can be expected ?\": \"video\",\n    \"What output do you expect ?\": \"LinkedIn Post\",\n    \"submittedAt\": \"2025-06-12T00:47:05.645+05:30\",\n    \"formMode\": \"test\"\n  },\n  {\n    \"Preferred tone or style for the LinkedIn post\": \"witty\",\n    \"submittedAt\": \"2025-06-12T01:15:11.608+05:30\",\n    \"formMode\": \"test\"\n  },\n  {\n    \"Should the post summarize the video or extract quotes?\": \"both\",\n    \"submittedAt\": \"2025-06-12T01:15:14.925+05:30\",\n    \"formMode\": \"test\"\n  },\n  {\n    \"Who is the target audience for the LinkedIn post?\": \"general network\",\n    \"submittedAt\": \"2025-06-12T01:15:20.045+05:30\",\n    \"formMode\": \"test\"\n  }\n]\n</inputs>\n\n<tools>\nYou do not have access to APIs, databases, or external documents. Use only the input provided.\n</tools>\n\n<instructions>\n1. Parse and extract all user-provided values from the JSON array.\n2. Understand the user’s goal, expected inputs and outputs, and key contextual details.\n3. Using that information, generate a final prompt in strictly the following format (Critics) where r and c will change the position r first and then c:\n\n- **<constraints>**: Any boundaries (length, style, tone, technical limits)\n- **<role>**: What the downstream AI agent’s expertise and purpose should be  \n- **<inputs>**: What inputs it will receive, in what format, and example values  \n- **<tools>**: Any tools or data sources it can or cannot access  \n- **<instructions>**: Step-by-step guidance for the agent to perform its task  \n- **<conclusions>**: What kind of output it should generate, with format or examples  \n\n4. Ensure the final prompt is useful for a general-purpose LLM, without ambiguity.\n</instructions>\n\n<constraints>\n- Always include all 6 sections: Role, Inputs, Tools, Instructions, Constraints, Conclusions\n- Be specific and concise, avoid generic phrasing\n- Do not include timestamps or metadata like \"formMode\" or \"submittedAt\"\n- Output must be readable by a prompt engineer or AI agent directly\n</constraints>\n\n<conclusions>\nYour output will be a complete structured prompt, ready to be used by a downstream LLM for task execution.\n\nExample output:\n<role>\nYou are an AI assistant that transforms short videos into compelling LinkedIn posts. Your job is to summarise the video, extract powerful quotes, and write in a witty tone suitable for a general professional audience.\n</role>\n\n<inputs>\nYou will receive:\n- A video (maximum 5 minutes)\n- Preferences for tone: witty\n- Summary style: both (summarize and extract quotes)\n- Target audience: general network\n</inputs>\n\n<tools>\nYou do not have access to external APIs or web search. You can assume the video has already been transcribed for processing.\n</tools>\n\n<instructions>\n1. Parse the video transcript and understand its core message.\n2. Identify key insights and at least one memorable quote.\n3. Write a LinkedIn post that begins with a strong hook, reflects a witty tone, and engages the general network.\n4. Balance insight and personality while staying platform-native.\n</instructions>\n\n<constraints>\n- Keep the post under 3000 characters\n- Avoid technical jargon unless it serves the audience\n- No generic intros or robotic tone\n</constraints>\n\n<conclusions>\nReturn a single, polished LinkedIn post. Example:\n\n---\n“Most products don’t need onboarding. They need rethinking.”\n\nJust watched a great clip on UX that reminded me how design isn’t about making things easier — it’s about making them unnecessary.\n\n#UX #DesignThinking\n---\n</conclusions>\n\n<output>\nReturn strictly only a JSON object like this:\n{\n  \"prompt\": \"<your generated prompt string>\"\n}\nDo NOT wrap it inside code blocks or markdown.\n</output>"
            }
          ]
        },
        "promptType": "define",
        "hasOutputParser": true
      },
      "executeOnce": true,
      "typeVersion": 1.6
    },
    {
      "id": "869e9a51-0e04-4bdc-8cf3-b35573b2953b",
      "name": "Google Gemini Chat Model1",
      "type": "@n8n/n8n-nodes-langchain.lmChatGoogleGemini",
      "position": [
        760,
        360
      ],
      "parameters": {
        "options": {},
        "modelName": "models/gemini-2.0-flash"
      },
      "credentials": {
        "googlePalmApi": {
          "id": "9BZpt0x33yMhJWqO",
          "name": "Google Gemini(PaLM) Api account 2"
        }
      },
      "typeVersion": 1
    },
    {
      "id": "cef87b06-dfd2-49ee-a294-75d3eabee58d",
      "name": "Sticky Note",
      "type": "n8n-nodes-base.stickyNote",
      "position": [
        -1220,
        380
      ],
      "parameters": {
        "width": 900,
        "height": 300,
        "content": "# Prompting\n\n- Constraints/Rules - [rules I need to abide by] - Defines boundaries, limitations, and guidelines for operation \n- Role/Scope - [what am I an expert of?] - Establishes the agent's purpose, identity, and overall objective \n- Inputs - [tell me what inputs I'm receiving] - Specifies expected data formats & parameters (inc. examples)\n- Tools - [what resources can I access? e.g. web search] - Outlines available resources, functions, and capabilities\n- Instructions/Tasklist - [order of tasks] - Provides step-by-step procedures with examples\n- Conclusions/Outputs - [what output am I providing (examples)] - Defines expected response formats and deliverables\n- Solutions/Error handling - [what do I do if I don't get the information I expected to?] - Addresses troubleshooting and exception\nmanagement|"
      },
      "typeVersion": 1
    },
    {
      "id": "cb8ee56d-7d41-4f37-a640-c8aea8588707",
      "name": "RelatedQuestionAI",
      "type": "@n8n/n8n-nodes-langchain.chainLlm",
      "position": [
        -700,
        -20
      ],
      "parameters": {
        "text": "={{ $json }}",
        "messages": {
          "messageValues": [
            {
              "message": "<role>\nYou are an expert LLM-based prompt refinement agent. Your goal is to analyze vague or semi-structured input from a user who wants to build an automation or AI-based tool. Based on what they share, your task is to generate 3 **highly specific** questions that, if answered, would help a prompt engineer craft a more tailored and effective prompt for the tool they wish to build. The questions you generate should be very specific to the ai agent the user wants to build, and completely relevant for the idea they want to build it for.\n</role>\n\n<input>\nYou will receive a JSON-like array with the following fields:\n- \"What do you want to build ?\" – Describes the general idea.\n- \"Tools I can access (N/A if no tools)\" – Lists any tools/services the user can integrate.\n- \"What Input can be expected ?\" – The user input or data source for the tool.\n- \"What output do you expect ?\" – The final result the tool should generate.\n- \"Any Constraints for the tool (N/A if no constraints)\" – Character/length/performance/time restrictions.\n\nEach field is plain text. The values may vary in clarity and depth.\n</input>\n\n<tools>\nYou do not have access to external tools. Only the given input array and your own reasoning ability are available. You cannot fetch additional context.\n</tools>\n\n<instructions>\n1. Parse and understand the user's goal.\n2. Identify any ambiguity or key gaps in what’s provided.\n3. Generate **3 clear, concise follow-up questions** that would best clarify:\n   - Context or tone expectations\n   - Format or structure needed\n   - Any target audience or usage specifics\n4. Explain **why** each question is important (in 1–2 sentences).\n5. Return your output in the strict JSON array format defined above.\n6. Identify missing but critical details that would affect how an AI agent should behave.\n7. For each missing detail, create one structured form field in the output format.\n8. Use fieldLabel for the question, placeholder to guide, and set requiredField appropriately.\n9. Optionally specify fieldType (e.g., textarea for long text, dropdown if fixed options are obvious).\n</instructions>\n\n<constraints>\n\nYour output must be in the following format:\n\n[\n  {\n    \"fieldLabel\": \"Label for the question to ask\",\n    \"placeholder\": \"Short hint to guide the user’s answer\",\n    \"requiredField\": true or false,\n    \"fieldType\": \"number\" | \"email\" | \"textarea\" | \"dropdown\" (not optional; take default as 'textarea')\n  }\n]\n\n- Ask no more than 3 questions.\n- Only ask questions that meaningfully impact how the tool would be built or how the AI would behave.\n- Your questions must be simple, not technical or abstract.\n- Do not repeat or rephrase questions already answered in the input.\n- Be practical — ask questions that a human prompt engineer would truly need to ask to make the result more useful.\n</constraints>\n\n<output>\n[\n  {\n    \"fieldLabel\": \"Preferred tone or style for the LinkedIn post\",\n    \"placeholder\": \"e.g., professional, friendly, witty\",\n    \"requiredField\": true,\n    \"fieldType\": \"textarea\"\n  },\n  {\n    \"fieldLabel\": \"Should the post summarize the video or extract quotes?\",\n    \"placeholder\": \"e.g., summary only, key quotes, both\",\n    \"requiredField\": true,\n    \"fieldType\": \"textarea\"\n  },\n  {\n    \"fieldLabel\": \"Who is the target audience for the LinkedIn post?\",\n    \"placeholder\": \"e.g., hiring managers, founders, general network\",\n    \"requiredField\": false,\n    \"fieldType\": \"textarea\"\n  }\n]\n</output>"
            }
          ]
        },
        "promptType": "define",
        "hasOutputParser": true
      },
      "typeVersion": 1.6
    },
    {
      "id": "6e88dd2e-6aa3-46b1-ae4e-437fcdd7d909",
      "name": "SplitQuestions",
      "type": "n8n-nodes-base.splitOut",
      "position": [
        -280,
        -20
      ],
      "parameters": {
        "options": {},
        "fieldToSplitOut": "output"
      },
      "typeVersion": 1
    },
    {
      "id": "d38f8848-8409-4ab5-a983-b927baa47585",
      "name": "Auto-fixing Output Parser",
      "type": "@n8n/n8n-nodes-langchain.outputParserAutofixing",
      "position": [
        880,
        140
      ],
      "parameters": {
        "options": {}
      },
      "typeVersion": 1
    },
    {
      "id": "de385387-86c1-45a2-a750-4f4a9b70cb0c",
      "name": "Structured Output Parser1",
      "type": "@n8n/n8n-nodes-langchain.outputParserStructured",
      "position": [
        960,
        360
      ],
      "parameters": {
        "jsonSchemaExample": "{\n\t\"prompt\": \"this is the prompt\"\n}"
      },
      "typeVersion": 1.2
    },
    {
      "id": "9ba8e561-6052-4d5c-915b-ebd7eeb910ad",
      "name": "Sticky Note1",
      "type": "n8n-nodes-base.stickyNote",
      "position": [
        -1220,
        -160
      ],
      "parameters": {
        "width": 440,
        "height": 320,
        "content": "# Initiate and Get the Basic Questions"
      },
      "typeVersion": 1
    },
    {
      "id": "5730302d-6e4b-435c-8e51-43d389d3f065",
      "name": "Sticky Note2",
      "type": "n8n-nodes-base.stickyNote",
      "position": [
        -760,
        -160
      ],
      "parameters": {
        "width": 380,
        "height": 500,
        "content": "# Generate Relevant Questions"
      },
      "typeVersion": 1
    },
    {
      "id": "f8f6640c-e97a-44b1-87bc-687783541309",
      "name": "Sticky Note3",
      "type": "n8n-nodes-base.stickyNote",
      "position": [
        -320,
        -160
      ],
      "parameters": {
        "width": 960,
        "height": 500,
        "content": "# Ask question to the user"
      },
      "typeVersion": 1
    },
    {
      "id": "cc14b692-ccf5-4ad0-9f59-1ec4eee5adfa",
      "name": "Sticky Note4",
      "type": "n8n-nodes-base.stickyNote",
      "position": [
        660,
        -160
      ],
      "parameters": {
        "width": 520,
        "height": 680,
        "content": "# Prompt Generator System"
      },
      "typeVersion": 1
    },
    {
      "id": "b42d7917-d7b4-4427-8530-c541ea7c1cef",
      "name": "Sticky Note5",
      "type": "n8n-nodes-base.stickyNote",
      "position": [
        1220,
        -160
      ],
      "parameters": {
        "width": 300,
        "height": 320,
        "content": "# Sending the Prompt to User"
      },
      "typeVersion": 1
    },
    {
      "id": "3e44d786-2cb2-41d8-8568-d0c50dc98c55",
      "name": "SendingPrompt",
      "type": "n8n-nodes-base.form",
      "position": [
        1280,
        -20
      ],
      "webhookId": "9a0af1f5-3257-486c-ad6e-068a7c0f93ab",
      "parameters": {
        "options": {
          "customCss": ".card {\n\tposition: relative;\n\tmax-width: 500px;\n\tmargin: 20px auto;\n\tpadding: 20px;\n\tbackground: #fefefe !important;\n\tborder-radius: 12px;\n\tbox-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);\n\tfont-family: 'Courier New', monospace;\n\tcolor: #1f2937;\n\tfont-size: 16px;\n\tline-height: 1.6;\n\twhite-space: pre-wrap;\n}\n\n.header p {\n  text-align: left;\n}\n\n@media (max-width: 768px) {\n\t.card {\n\t\tmargin: 10px !important;\n\t\tpadding: 15px !important;\n\t\tfont-size: 14px;\n\t}\n}\n"
        },
        "operation": "completion",
        "completionTitle": "🎉 Here's your custom prompt",
        "completionMessage": "={{ $('PromptGenerator').item.json.output.prompt }}\n\n---------------------------\n\n📋 You can now copy and use it anywhere!"
      },
      "typeVersion": 1
    },
    {
      "id": "176312e6-c5e6-4cba-ab4a-c8aeb5ee1722",
      "name": "Sticky Note6",
      "type": "n8n-nodes-base.stickyNote",
      "position": [
        -1220,
        -300
      ],
      "parameters": {
        "color": 7,
        "width": 440,
        "height": 100,
        "content": "# 🚀 AI Prompt generator"
      },
      "typeVersion": 1
    }
  ],
  "active": true,
  "pinData": {},
  "settings": {
    "callerPolicy": "workflowsFromSameOwner",
    "executionOrder": "v1",
    "executionTimeout": -1
  },
  "versionId": "6cdac3f9-1238-49d1-b6a9-01e2a3a4f273",
  "connections": {
    "BaseQuestions": {
      "main": [
        [
          {
            "node": "RelatedQuestionAI",
            "type": "main",
            "index": 0
          },
          {
            "node": "MergeUserIntent",
            "type": "main",
            "index": 0
          }
        ]
      ]
    },
    "LoopQuestions": {
      "main": [
        [
          {
            "node": "MergeUserIntent",
            "type": "main",
            "index": 1
          }
        ],
        [
          {
            "node": "RelevantQuestions",
            "type": "main",
            "index": 0
          }
        ]
      ]
    },
    "SplitQuestions": {
      "main": [
        [
          {
            "node": "LoopQuestions",
            "type": "main",
            "index": 0
          }
        ]
      ]
    },
    "MergeUserIntent": {
      "main": [
        [
          {
            "node": "PromptGenerator",
            "type": "main",
            "index": 0
          }
        ]
      ]
    },
    "PromptGenerator": {
      "main": [
        [
          {
            "node": "SendingPrompt",
            "type": "main",
            "index": 0
          }
        ]
      ]
    },
    "RelatedQuestionAI": {
      "main": [
        [
          {
            "node": "SplitQuestions",
            "type": "main",
            "index": 0
          }
        ]
      ]
    },
    "RelevantQuestions": {
      "main": [
        [
          {
            "node": "LoopQuestions",
            "type": "main",
            "index": 0
          }
        ]
      ]
    },
    "On form submission": {
      "main": [
        [
          {
            "node": "BaseQuestions",
            "type": "main",
            "index": 0
          }
        ]
      ]
    },
    "Google Gemini Chat Model": {
      "ai_languageModel": [
        [
          {
            "node": "RelatedQuestionAI",
            "type": "ai_languageModel",
            "index": 0
          }
        ]
      ]
    },
    "Structured Output Parser": {
      "ai_outputParser": [
        [
          {
            "node": "RelatedQuestionAI",
            "type": "ai_outputParser",
            "index": 0
          }
        ]
      ]
    },
    "Auto-fixing Output Parser": {
      "ai_outputParser": [
        [
          {
            "node": "PromptGenerator",
            "type": "ai_outputParser",
            "index": 0
          }
        ]
      ]
    },
    "Google Gemini Chat Model1": {
      "ai_languageModel": [
        [
          {
            "node": "PromptGenerator",
            "type": "ai_languageModel",
            "index": 0
          },
          {
            "node": "Auto-fixing Output Parser",
            "type": "ai_languageModel",
            "index": 0
          }
        ]
      ]
    },
    "Structured Output Parser1": {
      "ai_outputParser": [
        [
          {
            "node": "Auto-fixing Output Parser",
            "type": "ai_outputParser",
            "index": 0
          }
        ]
      ]
    }
  }
}
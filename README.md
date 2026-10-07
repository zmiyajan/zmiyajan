```text
                                     #**++==+*#    %
                                #*+=+++++++++++++***#
                          %##*****+=***#******####*#%#
                       #*####**###%##%%%%%%%%%%%%%%##%##%
                    %#*#######%%%%%%%%%%@@@%%%%%%%@@@%#%####
                  #*###%%%%%%%%%%%%%@@@%%%%%@@%%%%%%%@@%##%%##%
                **#%%%%%%%%%%%%%%%@@@@@@@@@%%###############%%%%
              #*##%%%%%%%#%%%%%%%%%%%@@@@%%##***++++========+*%%%%
             %*##%@%#*+==---==+++**####****+++====-----:::::--+#%%#
            %###%%#+------=========++++++++++==========--------+#%%##
            ###%%*=----==+++******++++++++++++++++++++++++===--=*#%%#%
           ##%%%#+----=++********+++++++====+++++++++++++++===--=*##%%
           %%%%#*+----=++++++======---==----===================--=##%%%
           %%%%#*+=--===++=====------------------------------=====*#%%%
           @@%%#*====----------========-------=====------:::::-===*##%%%
           @@%%#+===--:-+*###%%%%%%%##**+++++*#%%%%######***+=--===#%%%@
           @@%%*=----=*%%%%%#######%%%%%##**#%%%@@%%%%%%#######*=-==%%@
           @@%%+---=+**++++**###########**+*+*#%%%%%###****++++**=--*@@
           %@%#-:-=+++*#%%@%@@@@@*%@@%%%#+-::=*%%@@@@@@@@%%@@%#**+--=%@
        %*+*#%#::-==+*#%%%##%%%%%###%###*=:::-+##%%%%%%##########+===##+%
        %##**#+::----==++*###%%%%%%#****+=:::-=+**##%%%%%###*++======+#%#
        %%***#+---:::---===++**+++==++++=-:::-=++++=========-------==+#%#
         %+#%%+==--:::------:::::::-=+=-:::::::-=+==-:::::..::::---=+*##
          +#%%#+=--:::::::::::.:::-==-:::::-::::-:-=+=-:::::::::::-=+*#%
          #--*%#+=----:::::--::--=++-=+*+======***+=**+==---:::::--=+#+
          #---%%#+==--------=--==++++#%%%#+++*#%%#*==*##*+========++*%-
           #++#%%*+++=+========+++===+*#%%%%%%%%%*+=-=*#%%#**+*+***+*#*
               %%#******++==++###%%#*#%%@@%%##%%##***%%%%%%%##**##**#
                %****+***+++*%%@@@@%#****###**##%###%%@@@@@%#***###*%
                @#*++*##**+*#%@@@@@%%%######***+===+***##%%%########
                 %%*#**#%#**#%%###*++==++*#####**+==--===*#%%%%%###%
                 %%%%#*********++===---=+**#%%###*+======+*#%%%%#%@
                 #*%%%%%%######*=-------==+*##*++==-----=*#%%%%%%
                 ++*%@%%%%%%%@%#*=-::::::::--=--::::::-=*%%%@@@@
                *++++*#%%%@@@@@%#++=----=--+***+======+*%%%@@@
         ##*=:.-=+*++++**%%@@@@%%%%#******+*#*##*#####%%%@@@
    #*=-==++=+=----=+++***###%%%@@@@@%%%%%%##%%%%@%%%@@%%%*
===+++++*+===+*++=-::-=+******####%%%%@@@@@@@@@@@%%%%%#*+=+
-----==+=-=++==+++=--:::-=+************##%########*++==---*

    _____   _                 __   __  ____               _
   /__  /  (_)_  ______ _____/ /  /  |/  (_)_  ______ _  (_)___ _____
     / /  / / / / / __ `/ __  /  / /|_/ / / / / / __ `/ / / __ `/ __ \
    / /__/ / /_/ / /_/ / /_/ /  / /  / / / /_/ / /_/ / / / /_/ / / / /
   /____/_/\__, /\__,_/\__,_/  /_/  /_/_/\__, /\__,_/_/ /\__,_/_/ /_/
          /____/                        /____/     /___/

             AI Engineer  ·  Agentic AI  ·  Product Builder
```

I build AI agents and the products around them, and I measure them before I ship.

---

#### Featured: [Masdar · مصدر](https://github.com/zmiyajan/masdar)

Arabic-first search, quoted answers and contract checking over Saudi regulations
(Labor Law, PDPL, Companies Law), as they are **in force** after amendments. Built for HR, legal
and compliance teams. Local models only: no LLM, no API key, nothing generated.

- **Search** in formal Arabic or Saudi dialect: BM25 with Arabic light stemming, multilingual-E5
  dense retrieval and a cross-encoder reranker. **nDCG@10 0.932** on 82 hand-written questions,
  **0.923 on dialect questions**.
- **Answers** quote the law's own sentence with its citation, or say none answers. It cannot
  hallucinate because it never generates text.
- **Contract checker**: rules as code pinned to the text in force, evaluated on clauses written
  by independent authors. A flagged violation was never wrong; the published recall is the blind
  one, not the flattering one.
- **Also**: an amendment-aware BEIR dataset, an MCP server for AI agents, FastAPI with an RTL web
  UI, ports and adapters enforced in CI, and ADRs for every decision.

#### Other work

| Project | What it is |
|---|---|
| [Kashkah · كشخة](https://github.com/zmiyajan/kashkah) | Graduation project: an AI wardrobe and stylist with Arabic chat, clothing analysis from a photo, outfit recommendations and virtual try-on (Next.js, FastAPI). |
| [immich-takeout-uploader](https://github.com/zmiyajan/immich-takeout-uploader) | Imports a Google Photos takeout into Immich: a single dependency-free Python file with integrity checks and seven languages. |

#### How I work

- Evaluation first: gold sets, blind test sets and regression gates in CI.
- Clean boundaries: a pure domain, ports and adapters, `mypy --strict`, high test coverage.
- Decisions written down: an ADR for every choice that is not obvious.

**Stack:** Python · FastAPI · PyTorch / sentence-transformers · BM25 · MCP · TypeScript · Next.js · PostgreSQL

**Contact:** [zm.sa](https://zm.sa)

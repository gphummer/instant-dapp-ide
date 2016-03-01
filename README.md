# instant-dapp-ide
Complete Dapp and Solidity development environment as docker image you can run from command line

INSTRUCTIONS  
&nbsp;  
1) Install Docker & open Docker terminal (on Mac)  
2) Use ~/src as your Dapp project folder or edit run-image.sh  
Then when you're ready...  
3) $ setup-port-fowarding.sh  
4) $ pull-latest-image.sh  
5) $ run-image.sh  

     ___           _              _     ____                      ___ ____  _____   
    |_ _|_ __  ___| |_ __ _ _ __ | |_  |  _ \  __ _ _ __  _ __   |_ _|  _ \| ____|  
     | || '_ \/ __| __/ _` | '_ \| __| | | | |/ _` | '_ \| '_ \   | || | | |  _|  
     | || | | \__ \ || (_| | | | | |_  | |_| | (_| | |_) | |_) |  | || |_| | |___ 
    |___|_| |_|___/\__\__,_|_| |_|\__| |____/ \__,_| .__/| .__/  |___|____/|_____|  
                                                   |_|   |_|                      
    
     Build 2016-02-29.1

     NOTE: tmux is used to maintain concurrent windows. In window 0 we are running
     testrpc, which is a dummy blockchain for testing and development. In window 1
     we are running c9.sh, which makes the Cloud9 IDE available in a Web browser
     on http://localhost:8181. You are in window 2, which is a great place to
     manage your Dapp. Note you can create a new window using ctrl-b c, and you
     can navigate to an existing window using ctrl-b <window>.

     GET STARTED
     $ cd /src                # make external source code folder current directory
     $ mkdir new-proj         # create new project folder
     $ cd new-proj            # make project folder current directory
     $ truffle init           # initialize a bare bones project!!!
     $ truffle test           # run project's unit tests
     $ truffle build          # build the whole dapp (inc. html, js...)
     $ truffle deploy         # stick compiled contracts on testrpc chain
     $ ctrl-b c               # create window 3...
     $ truffle serve          # serve Dapp for testing on http://localhost:8080
     $ ctrl-b 2               # return window 2

     TIPS
     -- Share your Cloud9 url with collaborators (via external IP)
     ---- Cloud9 supports real time shared editing of code
     -- If you prefer using the terminal we have installed VIM
     ---- Ready pimped with NerdTree and Solidity support
     -- SSH server is installed for sharing the command line
     ---- Pairs join tmux sessions using $ tmux a -t pair

     DOCS
     -- https://media.readthedocs.org/pdf/solidity/latest/solidity.pdf
     -- https://github.com/ConsenSys/truffle
     -- https://gist.github.com/MohamedAlaa/2961058 [tmux]
     
     Enjoy! Ping me with feature requests via https://twitter.com/dominic_w

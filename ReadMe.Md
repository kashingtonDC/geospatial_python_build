# Building python environment on new computer
Setup instructions for 2023 M2 Mac
By aakash, 1/18/2024

# Install python 3.12
https://www.python.org/downloads/

* Verify it worked
Open a command line and type
`python3`

# Install sublime text 
https://www.anaconda.com/download

# Setup ~/.zshrc to make terminal outputs prettier
https://ohmyz.sh/

# add the subl alias to ~/.zshrc to open sublime from the command line
`vi ~/.zshrc`
`i`
`alias subl="'/Applications/Sublime Text.app/Contents/SharedSupport/bin/subl'"`

# Edit the robbyrussell zsh theme to show full path and tree emoji
`subl ~/.oh-my-zsh/themes/robbyrussell.zsh-theme`

# Change the first line to: 
PROMPT="%(?:%{$fg_bold[green]%}%1{➜%} :%{$fg_bold[red]%}%1{➜%} )🌳 %{$fg[cyan]%}%~%{$reset_color%}"

# Install anaconda
https://www.anaconda.com/download

* Verify it worked
Open a command line and type
`which conda`

# Create conda environment 
Open a command line and type
`conda create --name wt_env python=3.9`

# Activate environment 
Open a command line and type
`conda activate wt_env`

you should now see `wt_env` prepended to your path 

# Install the packages we need for eligibility analysis 
Open a command line and type
`conda install geopandas`
`conda install geospatial -c conda-forge`

# Install some other stuff we need
`conda install xmltodict openpyxl`

That's it! 
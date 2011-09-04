##INTRO##
    **galaxy** is a vim plugin that generate schemes with colors.
    With this you get:
        5 built-in schemes.
        Generate scheme with only one color.
        Edit schemes in 5 colors.
        Simply generate 100+ schemes with colorname-list.
        Terminal (256/16/8) support with all schemes.
        StatusLine highlight with insert-enter.
        ...

    Take a glance: http://i54.tinypic.com/2vi5h04.png

    where to start:     

        :colorscheme galaxy
        :Galaxy

##Use:##
    Load galaxy~
        :colorscheme galaxy

    Open galaxy manager window~
        <leader>gll or :Galaxy

        Then you can choose/edit/generate/delete schemes in it.

    Generate new schemes~
        'gn'
        Input your scheme's name.
        Then choose a color as the schemes background. then press 'q'
        To quit the choosing window. The schemes auto generated.
        And you will got your scheme loaded immediately.

    Edit your schemes~
        Move cursor on the color you want to edit. 
        Then press 'e'
        Then choose your desired color for it.
        Press 'q' to quit the window. 
        And you will got the changed scheme loaded immediately.

    Generate schemes with colorlist~
        <leader>cl or :ColorVlist
        You will got a colorlist window opened with W3C standard colorname.
        Put cursor in it. Then press '<leader>gla'
        All the colorlist in it will be generated to schemes.
        Colorlist like 'COLORNAME #ffffff' will be processed.

    Delete schemes~
        move cursor in the galaxy window. 
        press 'dd'.
        The scheme will be deleted.
    
    With Terminal~
        If it does not work correctly.
        You should check your '&t_Co' option.
        And set 'g:galaxy_term_color' to the number it support.


    NOTE    Your previous_scheme is cached on your disk.
            And gui scheme is seperated with terminal.
            So you can set them with different scheme.

    NOTE    Terminal scheme in 8/16 terminal color is predefined.

    NOTE    Terminal cursor may have bugs. 
            And only support "xterm\rxvt\screen\TMUX" now.

##Install:##
1.Using [Vundle.vim](Recommend):~
    https://github.com/gmarik/vundle
    After installed vundle and git. Add this line to your vimrc  
    `Bundle 'Rykka/vim-galaxy'` 
    `Bundle 'Rykka/ColorV'` 
    Run `:BundleInstall` to install.
    And update ColorV easily by `:BundleInstall!`
 
2.Using [Galaxy on Vim.org]~
 
    You should download latest 'ColorV' at first.
    http://www.vim.org/scripts/script.php?script_id=3597
    http://www.vim.org/scripts/script.php?script_id=3597
    Download the latest version of tar.gz file, 
    Extract to $VIMFILE folder. 
    ("~/.vim" for linux. "$HOME/vimfiles" for windows)
    Generate helptags. `:helptags ~/.vim/doc
 
    NOTE   Remember to install vim plugin 'ColorV' as forementioned.

    NOTE   You can always get the latest version at
           https://github.com/Rykka/vim-galaxy/
           And you can report bugs and suggestions at
           https://github.com/Rykka/vim-galaxy/issues 
        

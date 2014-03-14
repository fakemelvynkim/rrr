rrr(run run run) 
===

Run your script continuously for developing purposes! Execute rrr with your compiler, sleep time, and file you'd wish to run. Then, you'll see your script is executed continuously after the entered sleep time.



# MANUAL INSTALL

    # For OSX and Linux users
    git clone https://github.com/melvkim/rrr
    cd rrr
    sudo chmod +x rrr
    ln -s ./rrr /usr/local/bin

    # For Windows users
    echo "Please do the world a huge favor and quit using Windows." && shutdown -s now

# ONE-LINER INSTALL

TODO ADD install script using `curl` and `wget`

# EXAMPLE

    $date "+%Y/%m/%d, %H:%M:%S"
    2014/03/14, 02:46:44 
    $ls -A
    helloworld.rb
    $cat helloworld.rb
    puts 'rrr is a #1 must-have yet simplest developer tool for script-lovers!'
    $rrr ruby 10 helloworld.rb
    Execution time: 2014/03/14 02:46:44
    rrr is a #1 must-have yet simplest developer tool for script-lovers!
    
    Execution time: 2014/03/14 02:46:54
    rrr is a #1 must-have yet simplest developer tool for script-lovers!
    
    ^C
    $ls -A
    .20140314     helloworld.rb
    $ls -A ./.20140314
    024644.helloworld.rb
    $cat ./.20140314/024644.helloworld.rb
    Execution time: 2014/03/14 02:46:44
    rrr is a #1 must-have yet simplest developer tool for script-lovers!
    
    Execution time: 2014/03/14 02:46:54
    rrr is a #1 must-have yet simplest developer tool for script-lovers!
    
    $

# TODO
 - ADD other compilers

# VERSION
20140331.1

# vanilla.robotix.MikeSupplies
 Supplies packages for vanilla.robotix.MikeCore

# install GSL
Install from it: https://www.gnu.org/software/gsl/

./configure
make -j6
sudo make install

# resolve dependencies
rosdep install --from-paths ./src --ignore-packages-from-source --rosdistro melodic -y

# compile it
catkin_make_isolated

# add to ros environment
source ~/vanilla.robotix.MikeSupplies/devel_isolated/setup.bash

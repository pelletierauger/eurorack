# Copyright 2012 Emilie Gillet.
#
# This program is free software: you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation, either version 3 of the License, or
# (at your option) any later version.
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
# You should have received a copy of the GNU General Public License
# along with this program.  If not, see <http://www.gnu.org/licenses/>.

VERSION        = 0.1
F_CPU          = 32000000
MCU_NAME       = 32a4
TARGET         = edges_bootloader
PACKAGES       = avrlibx \
		avrlibx/io \
		avrlibx/system \
		avrlibx/utils \
		avrlibx/third_party/sp_driver \
		edges/bootloader
EXTRA_LD_FLAGS = ,--section-start=.text=0x8000,--relax

FUSE0 = 00
FUSE1 = 00
# bf enables the bootloader
FUSE2 = bf
FUSE4 = fe
FUSE5 = f7
LOCK = 3f

include avrlibx/makefile.mk

include $(DEP_FILE)

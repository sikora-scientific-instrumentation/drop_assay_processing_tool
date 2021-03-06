Drop-assay data-processing tool - PRE-RELEASE 2.1
----------------------------
Modified 11/6/21, S.Sikora: Correction of mistake in handling temperature edge-cases in fraction frozen table generation. (temperature, fraction_frozen_total) pairs that comprise the output table were sorted in temperature order to account for rare cases where the temperature series was not monotonically increasing. Adjacent entries with identical temperatures are then summed. However, this needs to be done with (temperature, fraction_frozen_this_frame) pairs, which are then converted to fraction_frozen_total following summation.

A python tool to assist in the processing and analysis of drop-assay data.

Installation instructions:
--------------------------

Python:
* Install Anaconda Python 3 (>= 3.8.5) - this will come with all the popular Python modules.

To run the tool:
--------------------

In the program directory, enter ipython drop_assay_processing_tool.py at the command line.
A short video demonstrating the use of the tool can be found [here](https://www.youtube.com/watch?v=IP2t19gC9Ec)

Licence:
--------

drop_assay_processing_tool is published under the terms of the GNU General Public License version 3. You should have received a copy of the GNU General Public License
along with drop_assay_processing_tool. If not, see <http://www.gnu.org/licenses/>.


(C) 2021 Dr Sebastien Sikora.
Sikora Scientific Instrumentation, Ipswich, UK.




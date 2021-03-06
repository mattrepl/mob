# Mob

A distributed workflow processing framework written in Clojure.

The goal of Mob is to provide distributed computing support to
data processing workflows with minimal configuration and management.  

Mob has two-levels of work distribution: nodes and mobs.

Nodes have jobqueues from which mobs reserve jobs.  Jobs
may be sent to a node through mob.jobqueue/put as well as a network interface (not implemented).
Mobs are implemented as a thread pool and individual threads process individual job requests.
Each mob has a message queue that stores received job messages and maintenance commands.


Mob's design was inspired by [Beanstalk](http://kr.github.com/beanstalkd/) and <del>Google's
MapReduce</del> functional programming's HOFs: map and reduce.

## Usage

Nothing worth using yet... 

## Installation

...or install, for that matter.

## License

Simplified BSD License

Copyright 2010 Matt Revelle. All rights reserved.

Redistribution and use in source and binary forms, with or without modification, are
permitted provided that the following conditions are met:

   1. Redistributions of source code must retain the above copyright notice, this list of
      conditions and the following disclaimer.

   2. Redistributions in binary form must reproduce the above copyright notice, this list
      of conditions and the following disclaimer in the documentation and/or other materials
      provided with the distribution.

THIS SOFTWARE IS PROVIDED BY <COPYRIGHT HOLDER> ``AS IS'' AND ANY EXPRESS OR IMPLIED
WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND
FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL <COPYRIGHT HOLDER> OR
CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

The views and conclusions contained in the software and documentation are those of the
authors and should not be interpreted as representing official policies, either expressed
or implied, of Matt Revelle.


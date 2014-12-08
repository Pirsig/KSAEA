Kerbal Space and Atmospheric Exploration Agency Tech Tree and Game Rebalance

So what is it?

This is a set of Module Manager configs designed to make the game a bit more challenging and to change the
tech tree progress into something more loosely realistic, starting with manned atmospheric flight and small,
unkerbaled, suborbital rockets.

I also wanted to match parts to nodes in a more logical way. Many parts have moved from their stock tiers and
nodes or stayed in the same tier but have changed nodes. Some nodes also have very few parts or only one when
not fleshed out with mods. This wasn't originally intentional, but I decided it made sense. Some breakthroughs
in science have very specific implications, some are very broad and far reaching.

I wanted to make use of the extra nodes at the end of the tree as well. If you're not aware, Squad has included
nodes at the end of the tree that require 1000 science to research, they do not show in R&D unless there's
actually parts assigned to them.  Not all of these nodes are used if you have just stock, but they continue to
flesh out as more mods are added.

Science has also been rebalanced a bit, but total science values are mostly no longer affected by this mod as
Squad added the functionality to change this in game with the difficulty settings introduced in .25. You get a
fair amount of science the first time doing an experiment (60% currently) with diminishing returns thereafter,
mimicking initial discovery and confirmation of scientific findings. Data amounts have also been reworked. This
was based on Science Revisited by CaptRobau, but most of the values have been reworked.

Sensor experiments like the temperature scan, now transmit 100% of their value. This will affect any mod part
using these modules as well. On the flip side of this, sample return type experiments like the mystery goo
experiment, have had their transmission values lowered even further to force either a proper return mission or
use of the lab. To go with this, the lab's boost to transmission value has been increased. The lab also consumes
more power during processing though and most sample return experiments will not transmit at quite 100% even
after processing.

Two new experiments have also been added. "Low Gravity Environment Experiments" are available on the Mobile
Processing Lab and provide science comparable to a seismic or gravity scan. It transmits at only 40% to
encourage you to process the experiment in the lab to get 100% transmission value. "Probe Situation Report" has
been added to all properly configured probe parts and provides a very small amount of science, even less than
crew reports. It does transmit at 100% however, and is meant to be the telemetry and operational data you're
ostensibly using to pilot the probe.

All the non shielded solar panels are no longer retractable to help give some differentiation. All solar panels
using the default squad module will now also use the curve created by CaptRobau in Science Revisited to follow
the inverse-square law.

SAS systems have been rebalanced to be far less powerful than their stock torque values.  This is to bring them
more in line with the real life use of SAS systems.  Currently this is a pretty basic across the board reduction
by 75% with a few specific tweaks here and there.  For instance, the 2.5m SAS part was hugely overpowered and so
has been further reduced.

Certain command parts have been deemed only for atmospheric flight.  If you only have stock parts this means only
the Mk1 series of cockpits.  These parts have had SAS removed entirely.  If you're using a life support mod these
parts will also not have any innate capacity to store the relevant resources.

This mod also adds several parts that are rescales and in a few cases, repurposing, of stock parts.  This is mostly
to help fill gaps at the beginning of the tree by adding more .625m parts.  Compatibility configs for mods that
provide similar parts will come in time and if you're using them instead, the parts created specifically for
filling this size gap are all in Parts/0625m Parts and you can feel free to delete them.

Additional Info

I approached this with a philosophy of wanting the mod to play nicely with other mods as much as possible.
Everything is done within the confines of the stock Squad defined tech tree, no new nodes have actually been
added or values for the nodes changed. While tree placement might be odd for parts in a mod I haven't made
configs for, nothing *should* break in any mod because of this one.

I've also tried to put together everything in such a way that it can be easily tailored to your personal needs,
separating different aspects of the pack into different configs so they can easily be removed individually.
They are also commented to be easily understandable and searchable for your own modification. All comments use
the part name displayed in game, allowing you to search for parts both by their actual part name as well as the
display name.

I started this without having any idea about Stupid_Chris' Stock ReBalance project, and originally had some of
the same things implemented alongside the tech tree rebalance.  This included solar panel changes, rebalancing
of probe cores, and a few other odds and ends.  As I was looking at getting deeper down the rabbit hole into
rebalancing many more parts, I found SRB which prompted me to remove most of that stuff from the mod and start
working specifically with SRB in mind.  I've since decided to back away from that idea and re-implemented many
of these original balance changes as well as expanded further.  

Because of MM run order, anything SRB does should run after me, so if your using SRB changes to the same
properties *should* take precedence over mine.  For the same reason, if you want to use SRB, but want my values
for say, SAS, you'd need to delete the relevant patches from SRB.  The compatibility for SRB provided with this
mod ONLY moves SRB's part rescales to appropriate nodes.  In the future I might offer a patch to run after SRB
and convert conflicting changes back to KSAEA values, but for now the only support I'm willing to commit in this
regard is assisting you in which parts of SRB to delete to get KSAEA values.

Why?

Because no other tech tree mod did what I actually wanted and Tree Loader seemed to be a complete mess to me.
Sure it functioned, but hitting an outside database, poor maintenance of the plugin, and it's eventual decline
into not being actively maintained left a very sour taste in my mouth. I'm grateful for many of the wonderful
plugins R4m0n built the foundation for, Tree Loader was a major miss for me though. There's plugins out there
now taking tree loader's place and they're fixing some issues, but I'd still have to rely on an unproven mod to
stay maintained.

On the other hand it's pretty clear Module Manager isn't going anywhere. It also has the lowest possibility for
any sort of conflict with another mod. Basically, the best way to make sure this plays nice with everyone's
setup is to use MM configs and type out a lot of stuff manually. Most mod authors already know how to use MM as
well and can easily make configs for their mods to follow this rebalance if they wish to do so without having
to learn anything extra really.

Taking this approach of not using any plugins outside MM itself does set certain limits. I can't modify EVA
kerbals for example, which is why they still transmit surface samples at the stock %. Though I've decided in
my head that the extra data is the kerbal's description of the sample . I also can't change the research values
for nodes in the tree or add new nodes, but honestly this just causes more room for compatibility issues. In
the end, it creates different approaches to a similar problem many of us have with not being satisfied with the
current tech/science setup and it's up to you which approach you like best.

Module Manager (http://forum.kerbalspaceprogram.com/threads/55219-Module-Manager) is required for this mod
to function and is included in the download.  Do not extract it if you have a more recent version.

INSTALLATION

1. Delete any previous version of KSAEA or older version of Module Manager.  
2. Unzip all contents to your Kerbal Space Program/GameData folder.

NOTE: If you're using this with an in progress save, any part you have already researched will still be
available to you, even if it's now moved to a node you've not researched.  This has to do with the way
the persistence file saves the parts you've unlocked and can be remedied by manually changing the
persistence file or starting a new game.  Deleting the moved parts, loading your save and causing it to
save a new tech tree without those parts, leaving the game, and restoring the parts, should also move
things to their proper place.

This rebalance builds on code and concepts from Science Revisted by Captrobau (http://forum.kerbalspaceprogram.com/threads/65033)

The Following mods have had compatability configs written:

Asmi's ECLSS Revived - http://forum.kerbalspaceprogram.com/threads/93328
Deadly Reentry Continued - http://forum.kerbalspaceprogram.com/threads/54954
DMagic Orbital Science - http://forum.kerbalspaceprogram.com/threads/64972
Interstellar Flight Inc. Life Support - http://forum.kerbalspaceprogram.com/threads/92011
Kerbal Attachment System - http://forum.kerbalspaceprogram.com/threads/92514
Procedural Fairings - http://forum.kerbalspaceprogram.com/threads/39512
Remote Tech - http://forum.kerbalspaceprogram.com/threads/83305
Snacks! Kerbal Simplified Life Support - http://forum.kerbalspaceprogram.com/threads/90841
Stock ReBalance - http://forum.kerbalspaceprogram.com/threads/75272
TAC Life Support - http://forum.kerbalspaceprogram.com/threads/40667
Universal Storage - http://forum.kerbalspaceprogram.com/threads/75129

License: CC BY NC SA
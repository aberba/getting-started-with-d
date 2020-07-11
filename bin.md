Resources for game developers
[YouTube channel by Ki Rill](https://www.youtube.com/playlist?list=PLgM-lc_kSqFQPF0UXgmFZpZalqcrSofe-) on beginner game development

> I'm talking about using the GC, but using it strategically. There are a number of ways to reduce pressure on the GC and minimize its impact on without dropping the benefits you get from the standard library, the runtime, and the GC itself. And they aren't onerous. Really, most of the people I see reaching first for betterC are throwing the baby out with the bathwater. There's no reason for it most of the time.

> D is not a managed language. The GC will only ever run a collection during an allocation, so you use the same strategy for allocation as you do in a C or C++ game engine: preallocate as much as possible, avoid allocations in your loops. See https://dlang.org/blog/the-gc-series/.

> According to success of Unity and my experience working with it having GC is actually great for game development but it is a no go for many core engine functionalities.

> Both the UE4 and Unity game engines use GC. Additionally, AAA games built with UE4 have shipped on consoles. UE4's GC certainly has issues (among other things), but you can still ship a game with it.

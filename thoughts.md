# Random Design Thoughts


Ideally we would like to deploy containers for our monitors and try to reuse a bunch of the existing faas infrastructure. 

Unfortunately software like docker adds a bunch of complexity to what we want. We dont need full isolated containers, we just want the packaging and ability to limit resources for them. We can add and remove namespaces as necessary. 

I propose we use raw runc containers to deploy monitors. This should be pretty easy for use to deploy monitors and have full control.

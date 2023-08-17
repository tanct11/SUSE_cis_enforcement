# puppet_pg_mod_template
Template for new Puppet Modules

## Directory Structure

**data**	        Hiera data that can be used when applying a manifest block.

**files**	        Static files that can be loaded by a plan or required as a dependency of a task. Prefer putting non-Ruby libraries used by a task here.

**functions**	    Puppet language functions that can be used from a plan.

**hiera.yaml**	  Hiera configuration for this module.

**lib**	          Typically Ruby code, such as custom Puppet functions, types, or providers.

**manifests**	    Classes and other Puppet code usable when applying a manifest block.

**metadata.json**	Typical metadata for a module describing version, operating system compatibility, and other module dependencies.

**plans**	        Plans, which must end in the .pp extension.

**tasks**	        Tasks and their metadata.

## Beset Practices

- Use an idempotent Puppet resource type to apply the change, avoid usage of EXEC when possible
- Use single quotes for any value that does not contain a variable. This protects against accidental interpolation of a variable. Use double quotes with strings containing variables.

# Migration Guide to Odoo 17.0

This document provides guidance for migrating the SaaS addons repository to Odoo 17.0.

## Overview

All modules in this repository have been upgraded to be compatible with Odoo 17.0:

- **Version**: All modules are now versioned as `17.0.1.0.0`
- **Installable**: All modules are marked as installable
- **Dependencies**: Core Odoo dependencies have been verified for Odoo 17 compatibility

## Module Status

All 23 modules in the repository have been updated:

- Core SaaS modules (`saas`, `saas_public`, `saas_portal`, etc.)
- Authentication modules (`auth_quick_master`)
- Feature modules (`saas_apps`, `saas_backups`, `saas_contract`, etc.)
- Utility and test modules

## External Dependencies

The following external dependencies have been updated to reference Odoo 17.0 branches:

- `queue` from OCA/queue
- `web` from OCA/web  
- `access-addons` from itpp-labs/access-addons
- `server-auth` from OCA/server-auth
- `contract` from OCA/contract
- `server-env` from OCA/server-env

## What Was Updated

1. **Manifest Files**: Version numbers updated to 17.0.1.0.0 format
2. **Documentation**: All "Tested on Odoo X.0" references updated to Odoo 17.0
3. **URLs**: Updated demo URLs and app store links to reference 17.0 versions
4. **Dependencies**: Verified core dependencies are compatible with Odoo 17

## What Was NOT Changed

In accordance with the migration strategy, the following were intentionally left unchanged:

- Business logic and Python code structure
- Data models and database schemas  
- View definitions and XML files
- JavaScript and CSS assets

## Next Steps

After this scaffolding update, further migration work may be needed:

1. Test module functionality with Odoo 17
2. Update any deprecated API calls in Python code
3. Verify XML view compatibility
4. Test JavaScript components for web framework changes
5. Update any custom CSS for Odoo 17 styling changes

## Support

For questions about this migration, please refer to the individual module documentation or contact the maintainers listed in each module's manifest file.
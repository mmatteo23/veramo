## API Report File for "@veramo/did-provider-web"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import { AbstractIdentifierProvider } from '@veramo/did-manager';
import { IAgentContext } from '@veramo/core';
import { IIdentifier } from '@veramo/core';
import { IKey } from '@veramo/core';
import { IKeyManager } from '@veramo/core';
import { IService } from '@veramo/core';

// @public
export class WebDIDProvider extends AbstractIdentifierProvider {
    constructor(options: {
        defaultKms: string;
    });
    // (undocumented)
    addKey({ identifier, key, options }: {
        identifier: IIdentifier;
        key: IKey;
        options?: any;
    }, context: IContext): Promise<any>;
    // (undocumented)
    addService({ identifier, service, options }: {
        identifier: IIdentifier;
        service: IService;
        options?: any;
    }, context: IContext): Promise<any>;
    // Warning: (ae-forgotten-export) The symbol "IContext" needs to be exported by the entry point index.d.ts
    //
    // (undocumented)
    createIdentifier({ kms, alias }: {
        kms?: string;
        alias?: string;
    }, context: IContext): Promise<Omit<IIdentifier, 'provider'>>;
    // (undocumented)
    deleteIdentifier(identifier: IIdentifier, context: IContext): Promise<boolean>;
    // (undocumented)
    removeKey(args: {
        identifier: IIdentifier;
        kid: string;
        options?: any;
    }, context: IContext): Promise<any>;
    // (undocumented)
    removeService(args: {
        identifier: IIdentifier;
        id: string;
        options?: any;
    }, context: IContext): Promise<any>;
}


```
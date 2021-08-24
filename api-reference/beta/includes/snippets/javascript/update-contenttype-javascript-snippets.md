---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80f06001bea1cd7b8c25428414a067c8a8dfab142fddf0b118cd17a1de1e87ac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903696"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contentType = {
    name: 'updatedCt',
    documentSet: {
        shouldPrefixNameToFile: true,
        allowedContentTypes: [{
            id: '0x0101',
            name: 'Document'
        }],
        defaultContents: [{
                fileName: 'a.txt',
                contentType: {
                    id: '0x0101'
                }
            },
            {
                fileName: 'b.txt',
                contentType: {
                    id: '0x0101'
                }
            }
        ],
        sharedColumns: [{
                name: 'Description',
                id: 'cbb92da4-fd46-4c7d-af6c-3128c2a5576e'
            },
            {
                name: 'Address',
                id: 'fc2e188e-ba91-48c9-9dd3-16431afddd50'
            }
        ],
        welcomePageColumns: [{
            name: 'Address',
            id: 'fc2e188e-ba91-48c9-9dd3-16431afddd50'
        }]
    }
};

await client.api('/sites/{site-id}/contentTypes/{contentType-id}')
    .version('beta')
    .update(contentType);

```
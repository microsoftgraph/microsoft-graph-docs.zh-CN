---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e6c39eb15298852ea36bdb615afc6cc102a13b7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773296"
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
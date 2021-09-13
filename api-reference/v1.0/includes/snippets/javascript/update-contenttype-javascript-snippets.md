---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7d25146afe11cf5c9307aedbc6a454bd386d83d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147537"
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
    .update(contentType);

```
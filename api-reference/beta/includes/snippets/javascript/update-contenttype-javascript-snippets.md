---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 271e3be8a60eed2b6e1d4c4b1e58d05267c0dbe2
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58516034"
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
      allowedContentTypes: [
         {
            id: '0x0101',
            name: 'Document'
         }
      ],
      defaultContents: [
         {
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
      sharedColumns: [
         {
            name: 'Description',
            id: 'cbb92da4-fd46-4c7d-af6c-3128c2a5576e'
         },
         {
            name: 'Address',
            id: 'fc2e188e-ba91-48c9-9dd3-16431afddd50'
         }
      ],
      welcomePageColumns: [
         {
            name: 'Address',
            id: 'fc2e188e-ba91-48c9-9dd3-16431afddd50'
         }
      ]
   }
};

await client.api('/sites/{site-id}/contentTypes/{contentType-id}')
    .version('beta')
    .update(contentType);

```
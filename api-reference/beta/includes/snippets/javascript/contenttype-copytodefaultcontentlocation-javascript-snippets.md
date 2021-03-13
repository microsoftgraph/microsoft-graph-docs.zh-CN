---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b80d516e11788c1a06d7366f8a13f44cbddd9166
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771076"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contentType = {
    sourceFile: {
        sharepointIds: {
            listId: 'e2ecf63b-b0fd-48f7-a54a-d8c15479e3b0',
            listItemId: '2'
        }
    },
    destinationFileName: 'newname.txt'
};

await client.api('/sites/{id}/contentTypes/{contentTypeId}/copyToDefaultContentLocation')
    .version('beta')
    .post(contentType);

```
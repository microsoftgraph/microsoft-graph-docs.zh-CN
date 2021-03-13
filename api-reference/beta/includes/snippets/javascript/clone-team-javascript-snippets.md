---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0a9ad258da336230b571392167fbbf6b27c5687
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799894"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const clone = {
     displayName: 'Library Assist',
     description: 'Self help community for library',
     mailNickname: 'libassist',
     partsToClone: 'apps,tabs,settings,channels,members',
     visibility: 'public'
};

await client.api('/teams/{id}/clone')
    .version('beta')
    .post(clone);

```
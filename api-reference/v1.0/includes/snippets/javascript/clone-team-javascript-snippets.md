---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0bf892dd06e249c2fe4f4d9da229c1f443c0c86c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781452"
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
    .post(clone);

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9bdb4c9731f642915e42a17f9d57df302d3ad91c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802482"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  displayName: 'displayName-value',
};

await client.api('/me/mailFolders/{id}/childFolders')
    .post(mailFolder);

```
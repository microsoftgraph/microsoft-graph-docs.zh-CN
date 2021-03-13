---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f699e14ef460130697a66afa32578c75478b63e4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799378"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  destinationId: 'destinationId-value'
};

await client.api('/me/mailFolders/{id}/copy')
    .version('beta')
    .post(mailFolder);

```
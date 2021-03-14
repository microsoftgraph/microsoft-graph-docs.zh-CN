---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ee6959da9601de21555ab8bcdc6bf8a6fcc1cca
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796840"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  displayName: 'Clutter'
};

await client.api('/me/mailFolders')
    .post(mailFolder);

```
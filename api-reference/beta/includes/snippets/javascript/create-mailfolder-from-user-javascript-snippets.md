---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7258ae2a85c5523c46dbd1feab0bd2f273c48ca4
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49661841"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  displayName: "Clutter"
};

let res = await client.api('/me/mailFolders')
    .version('beta')
    .post(mailFolder);

```
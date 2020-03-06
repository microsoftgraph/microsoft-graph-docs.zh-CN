---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5886ee3c3d022aeb6cbd7e9c0f3929bf9bc9322
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636826"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  displayName: "displayName-value",
};

let res = await client.api('/me/mailFolders/{id}/childFolders')
    .post(mailFolder);

```
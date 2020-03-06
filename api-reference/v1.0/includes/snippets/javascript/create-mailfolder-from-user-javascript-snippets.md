---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c95cc5d88c8b5dbf5c06b2aedf39f0ed506d25ec
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636741"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  displayName: "displayName-value"
};

let res = await client.api('/me/mailFolders')
    .post(mailFolder);

```
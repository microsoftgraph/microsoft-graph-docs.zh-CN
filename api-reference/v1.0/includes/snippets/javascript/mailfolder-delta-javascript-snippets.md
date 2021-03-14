---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2247410c14c9e8289e27903ac6a1b98f78319db
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793143"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/me/mailFolders/delta')
    .get();

```
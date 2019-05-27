---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cb205ccf55e5afe26b0a35d67c66e2061ba80c64
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34479131"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  displayName: "displayName-value",
};

let res = await client.api('/me/mailFolders/{id}')
    .update({mailFolder : mailFolder});

```
---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2cc759ff054dd5c2f9b76108ecbeed2a163d2d34
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463698"
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
    .version('beta')
    .post({mailFolder : mailFolder});

```
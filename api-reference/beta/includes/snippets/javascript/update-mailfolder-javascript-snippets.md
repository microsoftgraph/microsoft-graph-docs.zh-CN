---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ab2b39e47a53b810e353aada893cbbcebcdc786
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788393"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  displayName: 'displayName-value',
};

await client.api('/me/mailFolders/AAMkAGVmMDEzM')
    .version('beta')
    .update(mailFolder);

```
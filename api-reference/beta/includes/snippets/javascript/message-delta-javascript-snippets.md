---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2c1d2532f1f545d85dfd5720959aa8a07425a297
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478469"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/{id}/messages/delta')
    .version('beta')
    .get();

```
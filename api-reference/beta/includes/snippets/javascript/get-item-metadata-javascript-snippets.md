---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 07773e6296b594551f743825a42da1b651f4bf85
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35480154"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root')
    .version('beta')
    .get();

```
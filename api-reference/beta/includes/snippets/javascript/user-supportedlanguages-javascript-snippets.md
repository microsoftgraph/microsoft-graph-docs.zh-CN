---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 179b124b421c65dc2809f4c455e2c096a354587c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728842"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/supportedLanguages')
    .version('beta')
    .get();

```
---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 07773e6296b594551f743825a42da1b651f4bf85
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705897"
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
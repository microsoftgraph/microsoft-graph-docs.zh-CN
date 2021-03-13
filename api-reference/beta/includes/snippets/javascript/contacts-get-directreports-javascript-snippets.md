---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ae49ef4c2de26d17efc7b7bbede1450dcdc2a2c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797848"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directReports = await client.api('/contacts/{id}/directReports')
    .version('beta')
    .get();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 371a76d068f2fbce527bf628c4c8cf715cb800ba
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786484"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/connectors/{id}')
    .version('beta')
    .delete();

```
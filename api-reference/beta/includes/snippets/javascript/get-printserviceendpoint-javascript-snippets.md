---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 323ea0b8046d0f28ff9e5dd0b2097e7004f2fb20
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797374"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printServiceEndpoint = await client.api('/print/services/{id}/endpoints/{name}')
    .version('beta')
    .get();

```
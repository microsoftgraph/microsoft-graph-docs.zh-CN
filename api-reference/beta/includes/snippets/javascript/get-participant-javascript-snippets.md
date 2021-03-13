---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f8986b51a83b1edbcb11727022f95bd213ccf0e6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808722"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let participant = await client.api('/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants/7e1b4346-85a6-4bdd-abe3-d11c5d420efe')
    .version('beta')
    .get();

```
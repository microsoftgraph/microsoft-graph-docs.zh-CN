---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ba131d2d8e3a3c1ec6d93bfb6bde98dd4f607e0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781082"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printTaskDefinition = await client.api('/print/taskDefinitions/fab143fd-ee61-4358-8558-2c7dee953982')
    .version('beta')
    .get();

```
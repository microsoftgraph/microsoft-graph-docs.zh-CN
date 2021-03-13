---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a09ebb1df74763b5f2513c473f82ceed7a97092
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50768686"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printTaskDefinition = await client.api('/print/taskDefinitions/{printTaskDefinitionId}')
    .get();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f6c8d6e440900cacc76b7a8826d5dac10f01793
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776653"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let operations = await client.api('/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583/operations')
    .version('beta')
    .get();

```
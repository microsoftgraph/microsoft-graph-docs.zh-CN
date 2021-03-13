---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3cf724e04f0f7460b3fa09573c113642c48d0796
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785893"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const subscribeToToneOperation = {
  clientContext: 'fd1c7836-4d84-4e24-b6aa-23188688cc54'
};

await client.api('/communications/calls/{id}/subscribeToTone')
    .version('beta')
    .post(subscribeToToneOperation);

```
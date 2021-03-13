---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f949de4673cb7c6b2c1e0fc0612199459766f275
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780920"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let message = await client.api('/me/messages/AQMkADJmMTUAAAgVZAAAA/')
    .version('beta')
    .expand('mentions')
    .get();

```
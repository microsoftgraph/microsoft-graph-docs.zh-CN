---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 459c2a9bca9ef82fc4e08f26aabd178da29117b0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795753"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/messages/{id}')
    .version('beta')
    .delete();

```
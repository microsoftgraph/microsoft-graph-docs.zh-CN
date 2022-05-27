---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d62578f181fd552350c883b5d5df70fdfe8a96b
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719266"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const device = {
    extensionAttributes: {
        extensionAttribute1: 'BYOD-Device'
    }
};

await client.api('/devices/7c06cd31-7c30-4f3b-a5c3-444cd8dd63ac')
    .version('beta')
    .update(device);

```
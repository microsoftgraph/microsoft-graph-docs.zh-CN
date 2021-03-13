---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60cb46cf37c292c1c70a574eccf470c4442fd3ca
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785499"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groupLifecyclePolicy = await client.api('/groupLifecyclePolicies/{id}')
    .version('beta')
    .get();

```
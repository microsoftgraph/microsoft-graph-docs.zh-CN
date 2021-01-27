---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c142e4f6253b89ce9567b8a49c3f6817114272a4
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013624"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{userId}/usageRights')
    .version('beta')
    .filter('state in ('active', 'suspended') and serviceIdentifier in ('ABCD')')
    .get();

```
---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a1c45b6685ce48f5d0f3255388cac83b0afe487b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726254"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getYammerGroupsActivityGroupCounts(period='D7')')
    .version('beta')
    .get();

```
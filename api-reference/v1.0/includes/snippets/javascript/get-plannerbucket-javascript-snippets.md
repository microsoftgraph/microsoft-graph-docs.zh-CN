---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57e3301e2bbe01fd3b8d8d16b88f714025a97d74
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618721"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/buckets/{bucket-id}')
    .get();

```
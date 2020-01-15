---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8cc4a42af7ce974ad231ed46c0aaa526e3cdef0c
ms.sourcegitcommit: 5f643d3b3f71a9711963c8953da2188539fc9b0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/14/2020
ms.locfileid: "41123116"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/buckets/{bucket-id}/tasks')
    .get();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fe68eb602730aaf202a9661bfcc4af153a07c87
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797983"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let buckets = await client.api('/planner/plans/{plan-id}/buckets')
    .get();

```
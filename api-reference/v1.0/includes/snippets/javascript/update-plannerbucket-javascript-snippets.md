---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd95c5c80defa56abb5c226fd221aac7e620e3e1de1180a65019c5a99827fb08
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218707"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerBucket = {
  name: 'Development'
};

await client.api('/planner/buckets/{bucket-id}')
    .update(plannerBucket);

```
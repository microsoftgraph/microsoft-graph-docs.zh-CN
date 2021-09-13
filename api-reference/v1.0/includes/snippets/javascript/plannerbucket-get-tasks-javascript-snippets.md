---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3edd59196827946256d8fb6ed8eb8457978ac4230566e196864f260bf45947e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162020"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tasks = await client.api('/planner/buckets/{bucket-id}/tasks')
    .get();

```
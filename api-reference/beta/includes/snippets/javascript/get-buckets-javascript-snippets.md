---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d2ae0e582e67ce68f04649c1a8efa3f4efe97c9e
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945589"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/buckets')
    .version('beta')
    .get();

```
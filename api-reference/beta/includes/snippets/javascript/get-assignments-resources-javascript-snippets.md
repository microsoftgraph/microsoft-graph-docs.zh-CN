---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1f374ca0068d37322646d2f96da8acd3a4a97d1
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60891003"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let assignments = await client.api('/education/classes/{id}/assignments')
    .version('beta')
    .expand('resources')
    .get();

```
---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7a729050198291e73dc1dc358c092f1f4b1f8782
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493001"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{siteId}/drive')
    .get();

```
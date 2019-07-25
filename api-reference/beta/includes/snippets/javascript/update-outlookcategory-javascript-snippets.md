---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ddbac2686d52d5249e94cfb8ec5f7363098382d5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720956"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookCategory = {
  color:"preset15"
};

let res = await client.api('/me/outlook/masterCategories/bac262b7-485d-4739-b436-e31467d64fac')
    .version('beta')
    .update({outlookCategory : outlookCategory});

```
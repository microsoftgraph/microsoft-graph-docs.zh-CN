---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ddbac2686d52d5249e94cfb8ec5f7363098382d5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499783"
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
---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ef056e74ac90300062cb0ec631d1a2b3b8e7aa66
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478947"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d')
    .version('beta')
    .get();

```
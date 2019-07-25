---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f4dfc5523670622366a145094e89a41538d725fc
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733059"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/masterCategories/de912e4d-c790-4da9-949c-ccd933aaa0f7')
    .get();

```
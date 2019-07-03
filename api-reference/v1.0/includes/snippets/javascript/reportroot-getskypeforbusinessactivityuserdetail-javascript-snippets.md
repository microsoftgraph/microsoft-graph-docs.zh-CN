---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 71272819900e464a04e52ed180dd505ee40f13c3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509194"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessActivityUserDetail(period='D7')')
    .get();

```
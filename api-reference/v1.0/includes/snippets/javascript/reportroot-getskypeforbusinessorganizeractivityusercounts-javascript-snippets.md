---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5d40b38a6de9edadba3a7f5254e5205836862c24
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734585"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessOrganizerActivityUserCounts(period='D7')')
    .get();

```
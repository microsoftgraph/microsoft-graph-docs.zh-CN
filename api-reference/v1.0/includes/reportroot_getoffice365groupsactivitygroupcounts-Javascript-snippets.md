---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 632e3e56d6225fc5449188305ced6ee7a5500a6b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34478746"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365GroupsActivityGroupCounts(period='D7')')
    .get();

```
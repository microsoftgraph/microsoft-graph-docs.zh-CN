---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8e23540d710e0c0559e50e5c2ee37f392bc68f0c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463373"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOneDriveActivityFileCounts(period='D7')')
    .get();

```
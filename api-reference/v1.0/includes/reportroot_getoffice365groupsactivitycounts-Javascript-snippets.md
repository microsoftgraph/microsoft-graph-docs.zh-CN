---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4b4e18b2d91bf2b9860ca7b0134d3d344e32a113
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454206"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365GroupsActivityCounts(period='D7')')
    .get();

```
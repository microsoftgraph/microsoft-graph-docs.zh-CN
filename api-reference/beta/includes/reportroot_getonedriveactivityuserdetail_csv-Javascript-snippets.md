---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dcbb978c2ed2a22f9b7c9dd15fea3c7562b3ef27
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441127"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOneDriveActivityUserDetail(period='D7')')
    .version('beta')
    .get();

```
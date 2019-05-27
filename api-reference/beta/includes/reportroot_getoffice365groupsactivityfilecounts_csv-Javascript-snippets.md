---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5a35f480a88639511473d39074a24adb7a7dc7c9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441435"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365GroupsActivityFileCounts(period='D7')')
    .version('beta')
    .get();

```
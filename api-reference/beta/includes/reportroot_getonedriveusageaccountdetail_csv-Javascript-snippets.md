---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 11cde529aaa743e5e21e988cd85a695a314cdb6a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440994"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOneDriveUsageAccountDetail(period='D7')')
    .version('beta')
    .get();

```
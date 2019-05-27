---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7b2ba180bd8e4e0804880ba8c4e20e6300cecefb
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441302"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365GroupsActivityStorage(period='D7')')
    .version('beta')
    .get();

```
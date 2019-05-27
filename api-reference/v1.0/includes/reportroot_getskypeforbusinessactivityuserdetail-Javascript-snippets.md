---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 71272819900e464a04e52ed180dd505ee40f13c3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34476947"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessActivityUserDetail(period='D7')')
    .get();

```
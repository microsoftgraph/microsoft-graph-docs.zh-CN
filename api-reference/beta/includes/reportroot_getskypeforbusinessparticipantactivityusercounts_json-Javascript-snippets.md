---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4e33dc08cd4de82c57a6534a781df43e0ee06789
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463937"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')')
    .version('beta')
    .get();

```
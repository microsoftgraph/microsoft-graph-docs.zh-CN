---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 312897298874ecf792d35b57789ab06109978edf
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457458"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')')
    .get();

```
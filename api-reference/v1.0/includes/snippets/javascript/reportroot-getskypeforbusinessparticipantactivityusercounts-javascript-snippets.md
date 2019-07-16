---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 312897298874ecf792d35b57789ab06109978edf
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738217"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')')
    .get();

```
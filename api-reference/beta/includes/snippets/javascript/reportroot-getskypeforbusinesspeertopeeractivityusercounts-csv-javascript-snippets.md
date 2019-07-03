---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dbb5aa9929e5e8fd1cabdc35434b297c0e3e0141
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520771"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')')
    .version('beta')
    .get();

```
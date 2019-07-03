---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6364e0c00d034109ea463bab9212bd86bcd6539a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521625"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessPeerToPeerActivityCounts(period='D7')')
    .version('beta')
    .get();

```
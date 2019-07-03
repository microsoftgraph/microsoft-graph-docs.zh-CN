---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0d9ea6add3dd56644a87b0b5c3100a07b5bba80d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467483"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessParticipantActivityCounts(period='D7')')
    .get();

```
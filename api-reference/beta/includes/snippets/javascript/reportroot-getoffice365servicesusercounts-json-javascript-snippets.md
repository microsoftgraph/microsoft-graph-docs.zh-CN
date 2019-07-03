---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 362a7841c68cc5b5ceb38e1b93a9d4e48fd75a18
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521404"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365ServicesUserCounts(period='D7')')
    .version('beta')
    .get();

```
---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8011b988e8440c14c312dd0533053f9e388c9d47
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35727219"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOneDriveActivityFileCounts(period='D7')')
    .version('beta')
    .get();

```
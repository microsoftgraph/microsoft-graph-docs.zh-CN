---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 362a7841c68cc5b5ceb38e1b93a9d4e48fd75a18
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441344"
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
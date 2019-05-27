---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 28d5a833750bc11cbb2437618afe5eb07718c3f4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34481665"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd')
    .get();

```
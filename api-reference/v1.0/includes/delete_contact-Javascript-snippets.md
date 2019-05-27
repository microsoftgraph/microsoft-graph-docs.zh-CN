---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5e5bbf1ea0f9af75e5f03a539150f6608e81b6f8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459454"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contacts/{id}')
    .delete();

```
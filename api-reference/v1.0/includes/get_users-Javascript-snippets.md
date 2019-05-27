---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d203eb57d70a48d391d7ae884084071a5e786530
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34476261"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users')
    .get();

```
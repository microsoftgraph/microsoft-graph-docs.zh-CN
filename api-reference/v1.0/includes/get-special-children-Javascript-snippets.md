---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 57473cbb142913cac15f7cc69b15304a822415f3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34476408"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/special/{special-folder-name}/children')
    .get();

```
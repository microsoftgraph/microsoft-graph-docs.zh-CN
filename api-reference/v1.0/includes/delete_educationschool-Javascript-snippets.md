---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ddf51878d130f5b4a3884147ae84190fde538f80
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459141"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/schools/{school-id}')
    .delete();

```
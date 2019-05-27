---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e3962b9ef30cb009b184db4c97ada3f157a6b3c3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449263"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/delta(token='1230919asd190410jlka')')
    .get();

```
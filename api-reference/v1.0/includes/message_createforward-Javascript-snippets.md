---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 454f962d528d78da0bd886fcbda879896d332993
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34455458"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}/createForward')
    .post();

```
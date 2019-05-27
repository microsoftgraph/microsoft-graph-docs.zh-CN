---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e5d3e45cae234a9131ce07b20cbb6e4a881f72b4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34455444"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}/createReply')
    .post();

```
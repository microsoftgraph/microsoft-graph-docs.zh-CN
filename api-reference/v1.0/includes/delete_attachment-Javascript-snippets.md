---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3eb47b24a9817ab36769678b240699889028a6a5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459670"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/{id}/attachments/{id}')
    .delete();

```
---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6d864e777c0f1bcb3e0a99f0d4ba9124f6552e3f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34470018"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/acceptedSenders')
    .get();

```
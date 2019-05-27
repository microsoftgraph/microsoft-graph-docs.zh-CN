---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a76a6b4a593649c1fdcccb496e5b19a8e24d4041
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34451901"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/resetUnseenCount')
    .post();

```
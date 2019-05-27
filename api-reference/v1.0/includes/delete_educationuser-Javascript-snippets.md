---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c7902d1d0e753970b05ad8645786cb1018461be6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459158"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/users/{user-id}')
    .delete();

```
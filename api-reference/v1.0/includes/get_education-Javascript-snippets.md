---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 559344d7ebef9e7db480d8c05644d2cd1b951554
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34479628"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education')
    .get();

```
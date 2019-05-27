---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2aaa1aabc060a947a5a805dc6505f800161ed5ed
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436010"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/pages/{page-id}')
    .version('beta')
    .get();

```
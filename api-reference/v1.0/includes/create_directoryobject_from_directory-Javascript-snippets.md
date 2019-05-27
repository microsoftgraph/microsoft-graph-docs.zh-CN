---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2899d5e46380611c0f266d35e0cc4d198289795b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34478368"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directory/deletedItems/{object-id}/restore')
    .post();

```
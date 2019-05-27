---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 18896734af886cd22028f37781b36293afdb1f2d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34479747"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains/{domain-name}/domainNameReferences')
    .get();

```
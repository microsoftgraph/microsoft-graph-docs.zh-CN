---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 905800b37af4b742e1547f943b1de6a76fa66a0e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465669"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const administrativeUnit = {
  displayName: "displayName-value",
  description: "description-value",
  visibility: "visibility-value"
};

let res = await client.api('/administrativeUnits/{id}')
    .version('beta')
    .update({administrativeUnit : administrativeUnit});

```
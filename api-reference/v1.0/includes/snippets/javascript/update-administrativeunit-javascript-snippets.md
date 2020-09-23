---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbae0ccee78561f278f20b91dc9ec08de0a0ffac
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223684"
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

let res = await client.api('/directory/administrativeUnits/{id}')
    .update(administrativeUnit);

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b03fbc203d4e2373ec63f6889ddf33cc734dc764
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66040922"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/directory/administrativeUnits/{id}/members/$ref')
    .get();

```
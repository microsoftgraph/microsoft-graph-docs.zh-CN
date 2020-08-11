---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b838a98e421592d1c45ee54daa0bbef7159f949f
ms.sourcegitcommit: ab36e03d6bcb5327102214eb078d55709579d465
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2020
ms.locfileid: "45224794"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices/{id}/registeredUsers/{id}/$ref')
    .version('beta')
    .delete();

```
---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 867146d91976e1beba55eb7bfd00924c7b0c426e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34453556"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  directoryObject: {
  }
};

let res = await client.api('/directoryRoles/{id}/members/$ref')
    .version('beta')
    .post({directoryObject : directoryObject});

```
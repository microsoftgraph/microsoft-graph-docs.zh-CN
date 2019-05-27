---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ecc360f08bc57f2417da3b3191f2f8312d89a74b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34448354"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/oAuth2Permissiongrants')
    .version('beta')
    .get();

```
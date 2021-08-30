---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84ce93b7bb3fc6d8a3e907df72ae1d3d4396c3b778893941981b707d07367073
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103951"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let memberOf = await client.api('/servicePrincipals/{id}/memberOf')
    .version('beta')
    .get();

```
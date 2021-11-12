---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78a2d194b30e495a08811d425e20db39e84a3276eabdd93e973b43d5354876c8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218887"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let ownedObjects = await client.api('/servicePrincipals/{id}/ownedObjects')
    .version('beta')
    .get();

```
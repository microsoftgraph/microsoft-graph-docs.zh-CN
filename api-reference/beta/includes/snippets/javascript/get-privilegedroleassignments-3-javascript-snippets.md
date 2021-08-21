---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b76a4053d89da0266fb298b6b37e77129ffc907ac1aa6f30c728c2116358098
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273957"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let privilegedRoleAssignments = await client.api('/privilegedRoleAssignments')
    .version('beta')
    .filter('isElevated eq true and expirationDateTime eq null')
    .get();

```
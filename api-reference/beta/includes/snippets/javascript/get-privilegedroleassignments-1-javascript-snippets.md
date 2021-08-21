---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6faedad83f81d3d79cb366e29ea450d909ba730bd2e6e42d031063a64f8851f9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273951"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let privilegedRoleAssignments = await client.api('/privilegedRoleAssignments')
    .version('beta')
    .get();

```
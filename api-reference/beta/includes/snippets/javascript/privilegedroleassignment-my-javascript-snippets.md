---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c4667886f38f44e4176c96a1d040c82bf148050135edcf516ff284683cd6a759
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902490"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let my = await client.api('/privilegedRoleAssignments/my')
    .version('beta')
    .get();

```
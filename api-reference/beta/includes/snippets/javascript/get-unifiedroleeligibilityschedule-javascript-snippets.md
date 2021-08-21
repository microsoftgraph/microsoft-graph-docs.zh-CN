---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb3e2df45f2297eafba0a3c829e7ca6a61d54b5d9ff8fb4be0dd3b0888229cd7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105495"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleEligibilitySchedule = await client.api('/roleManagement/directory/roleEligibilitySchedules/5cfd7709-7709-5cfd-0977-fd5c0977fd5c')
    .version('beta')
    .get();

```
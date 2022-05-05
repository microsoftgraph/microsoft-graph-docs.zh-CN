---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad6501b36e1fe62a689f6472b279240721ff0afc
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205148"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/roleManagement/directory/roleAssignmentScheduleRequests/filterByCurrentUser(on='principal')')
    .get();

```
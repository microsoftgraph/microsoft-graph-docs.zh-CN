---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e965ba1462609cbbec9d79fdc7f4560be44a8ff4
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205032"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/roleManagement/directory/roleEligibilitySchedules/filterByCurrentUser(on='principal')')
    .get();

```
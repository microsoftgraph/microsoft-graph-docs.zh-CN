---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8cd9ba8d19f57148ab38f21d569f8ccb92bc3da1
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63351168"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const administrativeUnit = {
    displayName: 'Greater Seattle District Technical Schools'
};

await client.api('/administrativeUnits/4d7ea995-bc0f-45c0-8c3e-132e93bf95f8')
    .version('beta')
    .update(administrativeUnit);

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a839c2984f0da44ecf3d555005eff7e0991b6724
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63351234"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const administrativeUnit = {
    displayName: 'Greater Seattle District Technical Schools'
};

await client.api('/directory/administrativeUnits/4d7ea995-bc0f-45c0-8c3e-132e93bf95f8')
    .update(administrativeUnit);

```
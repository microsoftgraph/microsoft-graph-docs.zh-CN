---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef97fc684fa56d1bb9540c71f11561ba4fb098e23db42d4a34d7555c73fd5084
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409112"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/devices/{id}/registeredOwners/{id}/$ref')
    .delete();

```
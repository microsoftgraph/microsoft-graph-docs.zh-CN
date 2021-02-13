---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c096e87c07ef175837198b8e9a559fca72e67b0
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176734"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  roles: ["read"]
};

let res = await client.api('/sites/{sitesId}/permissions/{permissionId}')
    .update(permission);

```
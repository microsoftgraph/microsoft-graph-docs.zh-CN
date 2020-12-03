---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c24c4f26dbacb4147ba59cfaa6bcfb1bceae725a
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524165"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permissionGrantConditionSet = {
  permissionType: "delegated",
  clientApplicationsFromVerifiedPublisherOnly: true
};

let res = await client.api('/policies/permissionGrantPolicies/{id}/includes')
    .post(permissionGrantConditionSet);

```
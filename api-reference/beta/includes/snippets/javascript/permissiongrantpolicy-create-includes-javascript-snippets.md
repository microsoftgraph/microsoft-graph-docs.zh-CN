---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b50a7ee8b5383d3223c0ae772e559faf280ca47705d8c11aaf247f45dde2d41b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215798"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permissionGrantConditionSet = {
  permissionType: 'delegated',
  clientApplicationsFromVerifiedPublisherOnly: true
};

await client.api('/policies/permissionGrantPolicies/{id}/includes')
    .version('beta')
    .post(permissionGrantConditionSet);

```
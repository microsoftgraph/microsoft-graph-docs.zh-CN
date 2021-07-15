---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db5d63b1b959c0e1e6804a2110b38403e7202e1d
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440473"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  '@odata.id': 'https://graph.microsoft.com/odata/groups(\'dc3d2ce5-7c5e-4dca-a0ef-2145bf6e53ef\')'
};

await client.api('/policies/mobileDeviceManagementPolicies/dc3d2ce5-7c5e-4dca-a0ef-2145bf6e53ef/includedGroups/$ref')
    .version('beta')
    .post(group);

```
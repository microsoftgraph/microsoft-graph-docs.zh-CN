---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fab0ad4cc5da42c18f7c199ae2b45d6903932836
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2021
ms.locfileid: "60780508"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  '@odata.id': 'https://graph.microsoft.com/odata/groups(\'1a9db3ab-0acf-4808-99ae-e8ed581cb2e0\')'
};

await client.api('/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups/$ref')
    .version('beta')
    .post(group);

```
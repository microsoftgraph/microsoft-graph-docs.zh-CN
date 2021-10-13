---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e11d9b65bc5b6f030a1583eb8e93e9abb52a7f5cb4e101ae609c6d1c1ca85d2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278929"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/permissionGrantPolicies/my-custom-consent-policy/includes/198d8d6b-ecf6-47bc-a3dd-eaa2fe0544c5')
    .version('beta')
    .delete();

```
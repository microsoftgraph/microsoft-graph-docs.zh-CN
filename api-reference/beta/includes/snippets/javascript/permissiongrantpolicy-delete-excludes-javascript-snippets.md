---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bad61f7619e0345f4adbd39627acf4a7da7b5e6f7b15ea3b833a539db44c76a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278932"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/permissionGrantPolicies/my-custom-consent-policy/excludes/6a846635-3e70-4a10-821e-512a0db93cbd')
    .version('beta')
    .delete();

```
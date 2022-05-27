---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb28d1813fc834d24d1fca7089a2759ea731dec451abf0395c0942bacfd30d65
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158672"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages/{id}/$ref')
    .version('beta')
    .delete();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dccf8d1a6c833c76e99e8df2033192d695a3f29aedf213a00b407a881f0099f4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902781"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}')
    .version('beta')
    .delete();

```
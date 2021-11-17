---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0213a4b8b52d83deb19def9e8c6c6cce1c242a26cf08d434cd432e4e864f61b9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104855"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connectedOrganization = await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/{id}')
    .version('beta')
    .get();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b085cf116870dbc4f3391ba8914ef0948fde8b9a3e7bc167bb9e4e3f6965e031
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104848"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let internalSponsors = await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/{id}/internalSponsors')
    .version('beta')
    .get();

```
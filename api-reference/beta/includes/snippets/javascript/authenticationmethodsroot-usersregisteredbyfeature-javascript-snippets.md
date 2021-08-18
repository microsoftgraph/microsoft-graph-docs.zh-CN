---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 325eab8b937439d50931775a18256f6b557e2a3c95c9d54bb5d60827378e090a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105059"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userRegistrationFeatureSummary = await client.api('/reports/authenticationMethods/usersRegisteredByFeature(includedUserTypes='all',includedUserRoles='all')')
    .version('beta')
    .get();

```
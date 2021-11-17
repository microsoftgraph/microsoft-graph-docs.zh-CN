---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 767b6e12e9052076858b6d5248f1aae5c9acab9b18e6e9424767293433f533e7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104850"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let externalSponsors = await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/{id}/externalSponsors')
    .version('beta')
    .get();

```
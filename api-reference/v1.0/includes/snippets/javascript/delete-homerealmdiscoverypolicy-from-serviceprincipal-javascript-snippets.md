---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c5ca53759e380b93e2d168237b42a86c1a2a843
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864118"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}/$ref')
    .delete();

```
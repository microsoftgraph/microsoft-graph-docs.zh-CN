---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6025f95d90eb20eb597527a2ee2952649db54e5
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863618"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/claimsMappingPolicies')
    .get();

```
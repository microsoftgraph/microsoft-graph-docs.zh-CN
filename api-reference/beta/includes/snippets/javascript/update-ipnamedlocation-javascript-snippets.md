---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2aed64cc4a8d9d071dc82a243caac74bfb3c9fc8
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062258"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const namedLocation = {
    @odata.type: "#microsoft.graph.ipNamedLocation",
    displayName: "Untrusted named location with only IPv4 address",
    isTrusted: false,
    ipRanges: [
        {
            @odata.type: "#microsoft.graph.iPv4CidrRange",
            cidrAddress: "6.5.4.3/18"
        }

    ]
};

let res = await client.api('/identity/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2')
    .version('beta')
    .update(namedLocation);

```
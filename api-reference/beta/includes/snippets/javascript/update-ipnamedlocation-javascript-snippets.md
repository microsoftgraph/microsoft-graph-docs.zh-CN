---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3da4ece9bbc0166553ac5503599131ffa81036ac
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938456"
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

let res = await client.api('/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2')
    .version('beta')
    .update(namedLocation);

```
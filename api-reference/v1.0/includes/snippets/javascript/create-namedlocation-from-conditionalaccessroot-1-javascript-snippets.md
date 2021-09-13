---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c3cde0a919cad77fd7beca9262c881c9db433496fa2e3c48013177033fb2455
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221444"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const namedLocation = {
    '@odata.type': '#microsoft.graph.ipNamedLocation',
    displayName: 'Untrusted IP named location',
    isTrusted: false,
    ipRanges: [
        {
            '@odata.type': '#microsoft.graph.iPv4CidrRange',
            cidrAddress: '12.34.221.11/22'
        },
        {
            '@odata.type': '#microsoft.graph.iPv6CidrRange',
            cidrAddress: '2001:0:9d38:90d6:0:0:0:0/63'
        }
    ]
};

await client.api('/identity/conditionalAccess/namedLocations')
    .post(namedLocation);

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7436bdee0987e081830807c82498b9b3d76cae2c46af1549c569a992e1b5a895
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220335"
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
    .version('beta')
    .post(namedLocation);

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4fb9ba8b7355052261d74fec71da8a7c4f77f7ff1d7d65eb800fbb81d3f47280
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903155"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let staffMembers = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffMembers')
    .version('beta')
    .get();

```
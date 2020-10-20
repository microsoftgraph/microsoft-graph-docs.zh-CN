---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c56cc4e70ae3a7024732f06ac19b7fd845208a38
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604144"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish')
    .version('beta')
    .post();

```
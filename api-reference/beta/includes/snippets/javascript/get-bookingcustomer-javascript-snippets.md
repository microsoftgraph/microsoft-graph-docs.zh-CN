---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0f34a9bdee4c232a3a679d3d8e54c744e73b365719c6479ba66ee8d66b79fe8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903835"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bookingCustomer = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a')
    .version('beta')
    .get();

```
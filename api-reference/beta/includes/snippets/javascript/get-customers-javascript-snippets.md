---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 900a0cd147c252900d6f4878220310f532b297beae8823c6d4fa784907e1f4b9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105833"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let customers = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers')
    .version('beta')
    .get();

```
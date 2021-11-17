---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92aca3c8e947cdad0db273c3acd4cd8c832c7d750fbad70feb55aab7f5c69698
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162122"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKqAAA=')
    .version('beta')
    .delete();

```
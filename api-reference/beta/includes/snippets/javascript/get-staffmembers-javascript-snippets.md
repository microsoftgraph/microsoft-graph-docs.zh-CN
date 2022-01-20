---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2b85bc9f5158c0eb7ce6806fd76ae459bf48be6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106931"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let staffMembers = await client.api('/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/staffMembers')
    .version('beta')
    .get();

```
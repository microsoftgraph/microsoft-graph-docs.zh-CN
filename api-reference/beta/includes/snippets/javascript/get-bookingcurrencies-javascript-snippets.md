---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eec4f7a4fd8ff183aa204cba55ba21e436a460a9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786197"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bookingCurrencies = await client.api('/bookingCurrencies')
    .version('beta')
    .get();

```
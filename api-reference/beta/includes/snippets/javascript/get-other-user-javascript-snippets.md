---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbd828b89275e2e637c26493716f4093516a8856
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402440"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}')
    .version('beta')
    .get();

```
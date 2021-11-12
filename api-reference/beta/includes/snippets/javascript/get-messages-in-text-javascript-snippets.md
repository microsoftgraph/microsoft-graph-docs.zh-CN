---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 731d0e9ddd0738eb4fec38165714549d69ce0e56a5dbb1d8b9630dfe45e1d77e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161828"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messages = await client.api('/me/messages')
    .version('beta')
    .header('Prefer','outlook.body-content-type="text"')
    .select('subject,body,bodyPreview,uniqueBody')
    .get();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63b4691f8a9c28e6f7bf11f4a95f9cd921879a118e5e4cf949ce5e3de0550b1e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904051"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let event = await client.api('/me/events/AAMkAGI1AAAoZDOFAAA=/')
    .version('beta')
    .header('Prefer','outlook.body-content-type="text"')
    .select('subject,body,bodyPreview')
    .get();

```
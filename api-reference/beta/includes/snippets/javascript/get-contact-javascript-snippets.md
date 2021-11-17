---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f21d7d86c7023895ece445524365c290f18e77c76dc65b72aa0f39cd0a8ca1a6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332522"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contact = await client.api('/me/contacts/AAMkAGI2THk0AAA=')
    .version('beta')
    .get();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2475dc95445a10ef8fc071d9678efe025fc54d257479ad3ca99368b199390ed1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106122"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/onlineMeetings/550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype')
    .version('beta')
    .delete();

```
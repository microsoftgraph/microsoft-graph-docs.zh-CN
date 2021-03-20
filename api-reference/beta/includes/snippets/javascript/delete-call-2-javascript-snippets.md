---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38b876cb6f7d5034b8642d62e967a7affc6ca1ef
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945983"
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
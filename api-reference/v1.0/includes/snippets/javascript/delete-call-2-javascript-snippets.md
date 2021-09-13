---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4fc9cd7d8286e03e479c4df233b33a827dccf849b1aee973430acd3fd6e75ca8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162965"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/onlineMeetings/550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype')
    .delete();

```
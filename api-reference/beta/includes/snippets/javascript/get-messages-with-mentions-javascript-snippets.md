---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3bc4170f9d098857529b27151ada7d9031579d21
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176993"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages')
    .version('beta')
    .filter('MentionsPreview/IsMentioned eq true')
    .select('subject,sender,receivedDateTime,mentionsPreview')
    .get();

```
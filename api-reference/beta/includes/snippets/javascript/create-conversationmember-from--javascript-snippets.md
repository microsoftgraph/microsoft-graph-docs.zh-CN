---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf5a2e0d81c22d3c944140b8395c49788853155b
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142439"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationMember = {
    @odata.type: "#microsoft.graph.aadUserConversationMember",
    roles: ["owner"],
    user@odata.bind: "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
};

let res = await client.api('/teams/{id}/members')
    .version('beta')
    .post(conversationMember);

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9734624e22f0e27152a3b88c7e323094aef4ab6d
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49944955"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationMember = {
  @odata.type:"#microsoft.graph.aadUserConversationMember",
  roles: ["owner"]
};

let res = await client.api('/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19:56eb04e133944cf69e603c5dac2d292e@thread.skype/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')
    .version('beta')
    .update(conversationMember);

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66f61a05cf72a81ff64af656632c8c02c8d4b7ac
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868094"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const presence = {
    ids: ["fa8bf3dc-eca7-46b7-bad1-db199b62afc3", "66825e03-7ef5-42da-9069-724602c31f6b"]
};

let res = await client.api('/communications/getPresencesByUserId')
    .version('beta')
    .post(presence);

```
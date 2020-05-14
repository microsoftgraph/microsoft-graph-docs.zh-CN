---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5d3e45cae234a9131ce07b20cbb6e4a881f72b4
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "35732192"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}/createReply')
    .post();

```
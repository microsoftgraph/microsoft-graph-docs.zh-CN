---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2a57783e6d7738cb5f41e4d1e840f21dacae6262
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34453360"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  isRead: "true",
};

let res = await client.api('/me/messages/{id}')
    .update({message : message});

```
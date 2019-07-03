---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2a57783e6d7738cb5f41e4d1e840f21dacae6262
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35510216"
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
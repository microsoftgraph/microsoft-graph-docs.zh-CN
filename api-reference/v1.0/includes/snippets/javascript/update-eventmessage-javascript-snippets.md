---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2a57783e6d7738cb5f41e4d1e840f21dacae6262
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740303"
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
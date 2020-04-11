---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ddf58074cdcad8b25d9b7197bf685cc9df4ece52
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636994"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const event = {
  isOnlineMeeting: true,
  onlineMeetingProvider: "teamsForBusiness"
};

let res = await client.api('/me/events/AAMkADAGu0AABIGYDaAAA=')
    .version('beta')
    .update(event);

```
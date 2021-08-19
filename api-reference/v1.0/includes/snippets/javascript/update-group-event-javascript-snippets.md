---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e14869f85e39da7dc43d949987678e3f3e1ff00beb2708bd2b1b0f54da842c88
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902959"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const event = {
  location: {
      displayName: 'Conf Room 2'
  }
};

await client.api('/groups/01d4ee64-15ce-491e-bad1-b91aa3223df4/calendar/events/AAMkADZlAAAAABERAAA=')
    .update(event);

```
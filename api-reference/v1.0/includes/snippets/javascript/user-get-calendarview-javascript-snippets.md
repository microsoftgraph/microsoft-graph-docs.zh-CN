---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 978d679ff97e55bd04d46eed3919cf0ab73d54ef
ms.sourcegitcommit: 5f643d3b3f71a9711963c8953da2188539fc9b0c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/14/2020
ms.locfileid: "41123102"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendarView?startDateTime=2020-01-01T19:00:00-08:00&endDateTime=2020-01-02T19:00:00-08:00')
    .get();

```
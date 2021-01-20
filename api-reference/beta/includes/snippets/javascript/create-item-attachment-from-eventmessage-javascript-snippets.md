---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58b500dab7b6c986db8e9ec102213557e46f5892
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910794"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  @odata.type: "#Microsoft.OutlookServices.ItemAttachment",
  name: "name-value",
  item: {
    @odata.type: "microsoft.graph.message"
  }
};

let res = await client.api('/me/events/{id}/attachments')
    .version('beta')
    .post(attachment);

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b998028d22e54bc520b618181bc82978face298
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "43511118"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const checkin = {
  comment: "Updating the latest guidelines"
};

let res = await client.api('/drives/{drive-id}/items/{item-id}/checkin')
    .post(checkin);

```
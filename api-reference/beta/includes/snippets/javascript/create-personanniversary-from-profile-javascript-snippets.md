---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3376a86f41a117440444d67de1b6c14065e5af9
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37996582"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personAnniversary = {
  type: "type-value",
  date: "datetime-value"
};

let res = await client.api('/me/profile/anniversaries')
    .version('beta')
    .post(personAnniversary);

```
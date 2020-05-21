---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 747b4611773dfa62d579682c99d3f7935488ca99
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774795"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/meganb@contoso.OnMicrosoft.com/calendars/AAMkADlAABhbftjAAA=')
    .version('beta')
    .get();

```
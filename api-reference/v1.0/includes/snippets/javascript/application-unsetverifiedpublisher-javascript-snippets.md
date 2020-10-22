---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07573be6f8ea13b945363cd93f3920cc126d257d
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635511"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications/{id}/unsetVerifiedPublisher')
    .post();

```
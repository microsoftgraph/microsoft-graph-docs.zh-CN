---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9270b7997c17b1f1706bb36119eb28620f6a88ad
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614777"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendarView/delta')
    .header('Prefer','odata.maxpagesize=2')
    .skiptoken('R0usmcCM996atia_s')
    .get();

```
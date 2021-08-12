---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f015316dad3aa45338372278c90d9d419920b0ae8e64eaa81c9cd663e75e947
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54177844"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendarView/delta')
    .header('Prefer','odata.maxpagesize=2')
    .get();

```
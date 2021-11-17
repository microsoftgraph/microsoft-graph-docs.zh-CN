---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf0deeb4972754e698d31fa3b00ae1fb07c03926e9f001b746a21449c11682ca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103753"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let participants = await client.api('/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants')
    .version('beta')
    .get();

```
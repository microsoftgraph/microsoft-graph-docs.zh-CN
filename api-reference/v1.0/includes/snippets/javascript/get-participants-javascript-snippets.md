---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34a719d6009d7592899eba7aff8bbc6e79ab20e6001f5e326cf456ce4aa92606
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333819"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let participants = await client.api('/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants')
    .get();

```
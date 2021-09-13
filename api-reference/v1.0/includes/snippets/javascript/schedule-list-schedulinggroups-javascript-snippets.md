---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0955d2d78845b3692895d128453a8d9cce216b10f32aeae436b6027ce2ca116e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277656"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schedulingGroups = await client.api('/teams/{teamId}/schedule/schedulingGroups')
    .get();

```
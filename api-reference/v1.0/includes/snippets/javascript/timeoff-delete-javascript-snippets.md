---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b6492cca457d8a9bb0933fc280554fd5d5d9df536fffb22f720cf57008ee96e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278196"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{teamId}/schedule/timesOff/{timeOffId}')
    .delete();

```
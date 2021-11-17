---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 927563e4242da52e38297914b559de626815c3b8dc3a40c8f768bc475baaf883
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328761"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerRoster = await client.api('/planner/rosters/6519868f-868f-6519-8f86-19658f861965')
    .version('beta')
    .get();

```
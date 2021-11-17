---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab4eabdcbe4a30311ee8a21fdbeeffe186d8df306a03a8593d163d3aae982f15
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220790"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/me/planner/all/delta')
    .version('beta')
    .get();

```
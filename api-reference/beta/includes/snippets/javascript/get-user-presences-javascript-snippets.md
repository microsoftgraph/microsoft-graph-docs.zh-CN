---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89ffa93ef63cb91cc99f97b2af9a6f2b7444ff174db739204e8b260522fb9784
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101375"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let presence = await client.api('/communications/presences/dc74d9bb-6afe-433d-8eaa-e39d80d3a647')
    .version('beta')
    .get();

```
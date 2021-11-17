---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cccadd7cf65669948f0f90ce62cab3f2f0e5fb1d2ca0fb294e610e52dae802e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903954"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let place = await client.api('/places/3162F1E1-C4C0-604B-51D8-91DA78989EB1')
    .version('beta')
    .get();

```
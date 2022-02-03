---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 040ee651bae5d115ea7955df2ba065412c331729
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343822"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamworkDeviceConfiguration = await client.api('/teamwork/devices/e19229ed-29ed-e192-ed29-92e1ed2992e1/configuration')
    .version('beta')
    .get();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f18312ef42fab8fc12a62be5b9e84383199f1586
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945707"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/871dbd5c-3a6a-4392-bfe1-042452793a50/shiftPreferences')
    .version('beta')
    .get();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1a106da2a7c5fc8fddc73611178b1c1d80db78e
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343324"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamworkDevice = await client.api('/teamwork/devices/0f3ce432-e432-0f3c-32e4-3c0f32e43c0f')
    .version('beta')
    .get();

```
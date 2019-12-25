---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4cec73a4f8c43572a9f0087cda8fed9f4cedd432
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638033"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/contacts/{id}/memberOf')
    .get();

```
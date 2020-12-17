---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12062c6800280d544a314b6969367ffc5e3730be
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692863"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}')
    .get();

```
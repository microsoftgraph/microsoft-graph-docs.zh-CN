---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c418288dcc263824add66cdff261841bf46de32
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781139"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryRole = await client.api('/directoryRoles/23f3b4b4-8a29-4420-8052-e4950273bbda')
    .get();

```
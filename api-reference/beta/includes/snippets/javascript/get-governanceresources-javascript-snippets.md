---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d7b75f85d78ae02b5fca9229b490c1f46dfefa1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782140"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let resources = await client.api('/privilegedAccess/azureResources/resources')
    .version('beta')
    .get();

```
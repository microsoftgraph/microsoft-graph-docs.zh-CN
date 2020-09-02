---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72f1fa0da2e3577834443f8e3cf1dd2f8816fb05
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330328"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a')
    .version('beta')
    .get();

```
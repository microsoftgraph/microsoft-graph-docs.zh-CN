---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c931ceea238e45990211e84b9725815b8f409117
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801732"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schools = await client.api('/education/me/schools')
    .get();

```
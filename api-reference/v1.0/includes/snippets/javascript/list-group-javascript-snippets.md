---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50ee3ce0ac105614df96860c5f5a86c782415749
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771594"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let allowedGroups = await client.api('/print/shares/{printerShareId}/allowedGroups')
    .get();

```
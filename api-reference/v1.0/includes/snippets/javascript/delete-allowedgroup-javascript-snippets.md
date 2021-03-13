---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 763b7e2dabcd11da65ff421b2eef45fec622528c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771706"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/shares/{printerShareId}/allowedGroups/{groupId}/$ref')
    .delete();

```
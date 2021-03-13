---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de010dc7025c38342809482a238186ae0df1088b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785241"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let outlookTaskFolder = await client.api('/me/outlook/taskFolders/AAMkADIyAAAAABrJAAA=')
    .version('beta')
    .get();

```
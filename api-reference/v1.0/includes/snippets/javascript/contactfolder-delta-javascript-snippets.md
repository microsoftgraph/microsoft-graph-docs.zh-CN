---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a99f3b8aa52f9b1307a83873035f0dbad17275bf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808417"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/me/contactFolders/delta')
    .header('Prefer','odata.maxpagesize=2')
    .get();

```
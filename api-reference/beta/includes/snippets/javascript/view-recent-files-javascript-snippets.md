---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca2002bdb928ba3ee9acf859f9c32ff34b590a5e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779633"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let recent = await client.api('/me/drive/recent')
    .version('beta')
    .get();

```
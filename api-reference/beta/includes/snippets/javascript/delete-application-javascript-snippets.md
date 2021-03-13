---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: efcd0c73da119d9a2c6dd387e866866779044a48
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779821"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/applications/{id}')
    .version('beta')
    .delete();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ce43fdd45559b3369b9b06f9d1550d419bf24a5
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615884"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/programControls/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
    .version('beta')
    .delete();

```
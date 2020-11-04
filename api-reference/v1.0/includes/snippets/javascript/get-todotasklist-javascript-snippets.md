---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1991fd3e0429147b1a6b6aca992918df8e7ea631
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904148"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/todo/lists/AAMkADIyAAAAABrJAAA=')
    .get();

```
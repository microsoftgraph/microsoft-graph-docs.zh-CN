---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1eee9c5757cc04bd58107e809ee3fdf2f0d7ed1c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793073"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/schools/{school-id}')
    .delete();

```
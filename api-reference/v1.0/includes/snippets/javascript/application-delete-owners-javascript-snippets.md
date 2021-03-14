---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20bf2cd92b9e2aaeb358fe1e52bedae2a4e9bf91
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785061"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/applications/{id}/owners/{id}/$ref')
    .delete();

```
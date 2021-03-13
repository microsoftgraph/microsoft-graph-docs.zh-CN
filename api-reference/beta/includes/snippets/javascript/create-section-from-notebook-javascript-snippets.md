---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f092058a7ae230ea793fefdf1841848f149aa67c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786916"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteSection = {
  displayName: 'Section name'
};

await client.api('/me/onenote/notebooks/{id}/sections')
    .version('beta')
    .post(onenoteSection);

```
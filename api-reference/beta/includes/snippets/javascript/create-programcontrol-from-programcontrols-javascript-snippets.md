---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6aaa3b39f1748765b3d7045c81cc25bb5f427ab
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795783"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const programControl = {
    controlId: '7e59d237-2fb0-4e5d-b7bb-d4f9f9129213',
    controlTypeId: '6e4f3d20-c5c3-407f-9695-8460952bcc68',
    programId: '7e59d237-2fb0-4e5d-b7bb-d4f9f9129213'
};

await client.api('/programControls')
    .version('beta')
    .post(programControl);

```
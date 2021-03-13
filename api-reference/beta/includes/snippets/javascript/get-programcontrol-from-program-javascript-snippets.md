---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f654a9985639763e993d512085cb16c0f3a9c66
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802036"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let controls = await client.api('/programs/673a7379-9c38-4f01-bd9d-4fda7260b807/controls')
    .version('beta')
    .get();

```
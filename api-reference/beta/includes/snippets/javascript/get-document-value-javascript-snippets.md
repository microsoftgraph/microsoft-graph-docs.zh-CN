---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07eddead17b291ff5c37312cf905336377bba93e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780723"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/print/printers/fcb0bc53-a446-41d0-bfc3-5c56cdbb0f2a/jobs/46140/documents/bd260b1a-044e-4ca6-afa9-17d9a587d254/$value')
    .version('beta')
    .get();

```
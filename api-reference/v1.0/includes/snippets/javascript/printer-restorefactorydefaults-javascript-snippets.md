---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 512fa27085da35a5305d596131d0fe8cda07b97c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771818"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/printers/{printerId}/restoreFactoryDefaults')
    .post();

```
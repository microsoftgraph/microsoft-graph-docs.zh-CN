---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 549feba62caf88c9e3af6eab565dfc7d80e3fc48
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797703"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/programControls/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
    .version('beta')
    .delete();

```
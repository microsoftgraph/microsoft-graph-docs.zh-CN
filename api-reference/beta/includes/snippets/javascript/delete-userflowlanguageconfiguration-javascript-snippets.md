---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cca5139383a32679110c5a6f6a50d8658799b8a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779164"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/b2cUserFlows/B2C_1_Customer/languages/es-ES')
    .version('beta')
    .delete();

```
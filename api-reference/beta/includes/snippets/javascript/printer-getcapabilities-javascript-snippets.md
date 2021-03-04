---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d38a035c61db69b8d221c4751d1b2c28854c342
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447685"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printerCapabilities = await client.api('/print/printers/{id}/getCapabilities')
    .version('beta')
    .get();

```
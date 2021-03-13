---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9fe61e92df722d97dd4b9a5d0dced1384c26700a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787881"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let serviceConfigurationRecords = await client.api('/domains/contoso.com/serviceConfigurationRecords')
    .version('beta')
    .get();

```
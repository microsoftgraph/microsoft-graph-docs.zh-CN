---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6599e581a570b57df935852f92eb28807e0fd5c3
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920463"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/identity/b2xUserFlows/B2X_1_Partner/languages/en/defaultPages/idpselections/$value')
    .get();

```
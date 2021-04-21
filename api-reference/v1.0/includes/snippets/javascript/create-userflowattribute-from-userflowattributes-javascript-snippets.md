---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 59e92fab8f12e217dd99269dea578448ff397359
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920844"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityUserFlowAttribute = {
  displayName: 'Hobby',
  description: 'Your hobby',
  dataType: 'string',
};

await client.api('/identity/userFlowAttributes')
    .post(identityUserFlowAttribute);

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e01063024e9e6a0cf80c9034e00b544c7a55ac8
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920773"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments/City')
    .version('beta')
    .delete();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac98da63fee76bd9575ab1077bcb30da15b962ea
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920501"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/b2cUserFlows/B2X_1_Partner/languages/en/overridesPages/selfasserted1_1/$value')
    .version('beta')
    .delete();

```
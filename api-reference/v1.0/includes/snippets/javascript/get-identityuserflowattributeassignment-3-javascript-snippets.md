---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 903f186720cb58fe5f68878ec96f65186cab9bb7
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920726"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityUserFlowAttributeAssignment = await client.api('/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments/City')
    .get();

```
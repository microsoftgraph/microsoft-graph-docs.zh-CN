---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31bf96f8a1484a86438833c48d6563c78b431ed5
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920727"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityUserFlowAttributeAssignment = await client.api('/identity/b2xUserFlows/{id}/userAttributeAssignments/{id}')
    .expand('userAttribute')
    .get();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44aac2909e5456863adae6a15769c298199afab7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963302"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityUserFlowAttributeAssignment = await client.api('/identity/b2cUserFlows/{id}/userAttributeAssignments/{id}')
    .version('beta')
    .get();

```
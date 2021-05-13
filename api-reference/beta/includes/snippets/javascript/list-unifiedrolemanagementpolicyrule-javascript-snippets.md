---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: deb11bb0052ec34454c35541e4e5a36b5ef29bdc
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474283"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let effectiveRules = await client.api('/policies/roleManagementPolicies/ba9cc2d6-c2d6-ba9c-d6c2-9cbad6c29cba/effectiveRules')
    .version('beta')
    .get();

```
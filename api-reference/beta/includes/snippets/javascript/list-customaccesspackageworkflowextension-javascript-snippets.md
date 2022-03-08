---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cee4c25870f17284129a49140f34c8bf3c4ac773
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338202"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let customAccessPackageWorkflowExtensions = await client.api('/identityGovernance/entitlementManagement/accessPackageCatalogs/32efb28c-9a7a-446c-986b-ca6528c6669d/customAccessPackageWorkflowExtensions')
    .version('beta')
    .get();

```
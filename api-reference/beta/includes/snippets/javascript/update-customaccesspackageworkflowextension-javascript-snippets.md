---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82daf9d47539c4421a754b33f4c9ab3a8c1e15a4
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338270"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const customAccessPackageWorkflowExtension = {
  '@odata.type': '#microsoft.graph.customAccessPackageWorkflowExtension',
  displayName: 'test_action_0124_email',
  description: 'this is for graph testing only'
};

await client.api('/identityGovernance/entitlementManagement/accessPackageCatalogs/32efb28c-9a7a-446c-986b-ca6528c6669d/customAccessPackageWorkflowExtensions/98ffaec5-ae8e-4902-a434-5ffc5d3d3cd0')
    .version('beta')
    .put(customAccessPackageWorkflowExtension);

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86a8e0d15ecda5ca882a6bd070157eebb3780141
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789348"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const assign = {
  '@odata.type': '#microsoft.graph.cloudPcProvisioningPolicyAssignment',
  assignments: [
    {
      id: 'b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff',
      target: {
        '@odata.type': 'microsoft.graph.cloudPcManagementGroupAssignmentTarget',
        groupId: '64ff06de-9c00-4a5a-98b5-7f5abe26ffff'
        }
    }
  ]
};

await client.api('/deviceManagement/virtualEndpoint/provisioningPolicies/{id}/assign')
    .version('beta')
    .post(assign);

```
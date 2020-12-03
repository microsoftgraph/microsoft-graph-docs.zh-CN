---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 214a626df43d2a1f0fb475024ee33a92b53cea4f
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521563"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const assign = {
  @odata.type: "#microsoft.graph.cloudPcProvisioningPolicyAssignment",
  assignments: [
    {
      id: "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff",
      target:{
        @odata.type: "microsoft.graph.cloudPcManagementGroupAssignmentTarget",
        groupId:"64ff06de-9c00-4a5a-98b5-7f5abe26ffff"
        }
    }
  ]
};

let res = await client.api('/deviceManagement/virtualEndpoint/provisioningPolicies/{id}/assign')
    .version('beta')
    .post(assign);

```
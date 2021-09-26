---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c2ef4ceb3cfb5ce7f75cc64817afb7a912b747dab7d5f95bc7ada0ecfd72663
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218511"
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
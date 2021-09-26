---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d291288352e0eb237c91c3fb953784fea131807ca541a112c7ac6b598b049a1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105812"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const assign = {
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

await client.api('/deviceManagement/virtualEndpoint/userSettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff/assign')
    .version('beta')
    .post(assign);

```
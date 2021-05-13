---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 87bc70567edf705880ff03b6490ba2d2a5fe542f
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475202"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleEligibilityScheduleRequest = {
  '@odata.type': '#Microsoft.Identity.Governance.Common.Data.ExternalModels.V1.unifiedRoleEligibilityScheduleRequest',
  action: 'String',
  principalId: 'String',
  roleDefinitionId: 'String',
  directoryScopeId: 'String',
  appScopeId: 'String',
  isValidationOnly: 'Boolean',
  targetScheduleId: 'String',
  justification: 'String',
  scheduleInfo: {
    '@odata.type': 'microsoft.graph.requestSchedule'
  },
  ticketInfo: {
    '@odata.type': 'microsoft.graph.ticketInfo'
  }
};

await client.api('/roleManagement/directory/roleEligibilityScheduleRequests')
    .version('beta')
    .post(unifiedRoleEligibilityScheduleRequest);

```
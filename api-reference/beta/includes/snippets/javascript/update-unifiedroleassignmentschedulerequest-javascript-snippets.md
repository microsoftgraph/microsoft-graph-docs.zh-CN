---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 574307edd7af12082e92924a22cacf09eeaa0f9f
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475475"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleAssignmentScheduleRequest = {
  '@odata.type': '#microsoft.graph.unifiedRoleAssignmentScheduleRequest',
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

await client.api('/roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}')
    .version('beta')
    .update(unifiedRoleAssignmentScheduleRequest);

```
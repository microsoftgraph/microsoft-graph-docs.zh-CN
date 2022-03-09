---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9f53b9a9eb8382b3a2b51f302c3e219d0468ce1
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63397727"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageAssignmentPolicy = {
  displayName: 'extension-policy',
  description: 'test',
  accessPackageId: 'ba5807c7-2aa9-4c8a-907e-4a17ee587500',
  expiration: {
    type: 'afterDuration',
    duration: 'P365D'
  },
  canExtend: false,
  requestApprovalSettings: null,
  requestorSettings: {
    acceptRequests: true,
    scopeType: 'AllExistingDirectorySubjects',
    allowedRequestors: [],
    isOnBehalfAllowed: false
  },
  accessReviewSettings: null,
  questions: [],
  customExtensionHandlers: [
    {
      stage: 'assignmentRequestCreated',
      customExtension: {
        id: '219f57b6-7983-45a1-be01-2c228b7a43f8' //customAccessPackageWorkflowExtension.id
      }
    },
    {
      stage: 'assignmentRequestGranted',
      customExtension: {
        id: '219f57b6-7983-45a1-be01-2c228b7a43f8'
      }
    }
  ]
};

await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies')
    .version('beta')
    .post(accessPackageAssignmentPolicy);

```
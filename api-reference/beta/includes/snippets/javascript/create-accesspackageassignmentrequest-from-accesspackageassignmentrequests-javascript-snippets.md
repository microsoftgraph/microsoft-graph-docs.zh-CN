---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb23e8b834f9b1a3f452438f5180e6844baf5743
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37992788"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageAssignmentRequest = {
  requestType: "AdminAdd",
  accessPackageAssignment:{
     targetId:"46184453-e63b-4f20-86c2-c557ed5d5df9",
     assignmentPolicyId:"2264bf65-76ba-417b-a27d-54d291f0cbc8",
     accessPackageId:"a914b616-e04e-476b-aa37-91038f0b165b"
  }
};

let res = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentRequests')
    .version('beta')
    .post(accessPackageAssignmentRequest);

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d8afeb03a77b9556ed84a2c0f4d92e43bd1d6c3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773856"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const legalHold = {
  '@odata.type': '#microsoft.graph.ediscovery.legalHold',
  description: 'String',
  createdBy: {
    '@odata.type': 'microsoft.graph.identitySet'
  },
  isEnabled: 'Boolean',
  status: 'String',
  contentQuery: 'String',
  errors: [
    'String'
  ],
  displayName: 'String'
};

await client.api('/compliance/ediscovery/cases/{caseId}/legalHolds')
    .version('beta')
    .post(legalHold);

```
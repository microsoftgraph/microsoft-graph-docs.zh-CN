---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d81ded0a94df85abfcbbcfb176dcaf00d19f7eae665ff7d6202ba6bfd52f9c2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902276"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationSchool = {
  '@odata.type': '#microsoft.graph.educationSchool',
  displayName: 'String',
  description: 'String',
  externalSource: 'String',
  externalSourceDetail: 'String',
  principalEmail: 'String',
  principalName: 'String',
  externalPrincipalId: 'String',
  lowestGrade: 'String',
  highestGrade: 'String',
  schoolNumber: 'String',
  externalId: 'String',
  phone: 'String',
  fax: 'String',
  createdBy: {
    '@odata.type': 'microsoft.graph.identitySet'
  },
  address: {
    '@odata.type': 'microsoft.graph.physicalAddress'
  }
};

await client.api('/education/schools')
    .post(educationSchool);

```
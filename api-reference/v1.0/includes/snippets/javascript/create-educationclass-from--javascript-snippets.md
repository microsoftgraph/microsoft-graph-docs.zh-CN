---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8c43a50d48574be7ad38df05bda5ea6c37499d5c9dec00df4c2d72a689dcab8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161623"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationClass = {
  '@odata.type': '#microsoft.graph.educationClass',
  displayName: 'String',
  mailNickname: 'String',
  description: 'String',
  createdBy: {
    '@odata.type': 'microsoft.graph.identitySet'
  },
  classCode: 'String',
  externalName: 'String',
  externalId: 'String',
  externalSource: 'String',
  externalSourceDetail: 'String',
  grade: 'String',
  term: {
    '@odata.type': 'microsoft.graph.educationTerm'
  }
};

await client.api('/education/classes')
    .post(educationClass);

```
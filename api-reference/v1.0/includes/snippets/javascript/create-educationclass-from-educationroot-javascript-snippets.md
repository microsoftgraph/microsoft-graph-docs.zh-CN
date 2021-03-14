---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8abd43730142a41888aa8bf503abcb8e433af087
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785395"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationClass = {
  description: 'Health Level 1',
  classCode: 'Health 501',
  displayName: 'Health 1',
  externalId: '11019',
  externalName: 'Health Level 1',
  externalSource: 'sis',
  mailNickname: 'fineartschool.net'
};

await client.api('/education/classes')
    .post(educationClass);

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e06af17ac142b0deeb8664c8bd0a847c409ff0a00300d1377d14aa0f97323682
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161270"
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
    .version('beta')
    .post(educationClass);

```
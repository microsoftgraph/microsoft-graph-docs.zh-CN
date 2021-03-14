---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3eff5d43b08fcaaf95bd4a3fbff8055dd1e594ef
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797662"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  description: 'description-value',
  displayName: 'displayName-value',
  groupTypes: [
    'groupTypes-value'
  ],
  mail: 'mail-value',
  mailEnabled: true,
  mailNickname: 'mailNickname-value'
};

await client.api('/groups/{id}')
    .update(group);

```
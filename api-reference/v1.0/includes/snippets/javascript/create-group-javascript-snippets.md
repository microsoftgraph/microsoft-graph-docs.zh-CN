---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e420683165b2d0c038a6b511ba0db9b3c88b978
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806076"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  description: 'Self help community for library',
  displayName: 'Library Assist',
  groupTypes: [
    'Unified'
  ],
  mailEnabled: true,
  mailNickname: 'library',
  securityEnabled: false
};

await client.api('/groups')
    .post(group);

```
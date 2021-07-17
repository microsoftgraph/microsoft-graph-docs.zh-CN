---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ebc410f87be4d7a9efb7185dbc1163a3a742200
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53444932"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  description: 'Library Assist',
  displayName: 'Library Assist',
  groupTypes: [
    'Unified'
  ],
  mailEnabled: true,
  mailNickname: 'library-help'
};

await client.api('/groups/{id}')
    .update(group);

```
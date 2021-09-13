---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a3883b8a9bd910e5c699eaf979b8d63c87480e7851ef189f35556e1c254ac03
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106432"
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
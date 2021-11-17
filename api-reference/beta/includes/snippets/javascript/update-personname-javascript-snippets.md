---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4488677bebae8f1f353d6a24f784900657c82350793fd166d87927d7cdae726
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219861"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personName = {
  nickname: 'Kesha'
};

await client.api('/me/profile/names/{id}')
    .version('beta')
    .update(personName);

```
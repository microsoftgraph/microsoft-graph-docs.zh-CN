---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0df1a9e44251616ce61f8305dbff1c451190a7f9f2db97d9c6d5b93a4cebe71f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219750"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/owners/{id}/$ref')
    .version('beta')
    .delete();

```
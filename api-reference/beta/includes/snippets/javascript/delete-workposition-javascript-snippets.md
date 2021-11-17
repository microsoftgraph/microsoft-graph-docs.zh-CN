---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae7bb0a18ff4b22fce1afb679cd5a252416ee2252a6f5b655c9727ba03089451
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163198"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/profile/positions/{id}')
    .version('beta')
    .delete();

```
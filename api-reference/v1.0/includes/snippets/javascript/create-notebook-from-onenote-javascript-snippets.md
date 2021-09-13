---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6b6fd0e5b420490cb7cbd15860bdd5a69560c44d02ffdb025976261283f4011
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278339"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const notebook = {
    displayName: 'My Private notebook'
};

await client.api('/me/onenote/notebooks')
    .post(notebook);

```
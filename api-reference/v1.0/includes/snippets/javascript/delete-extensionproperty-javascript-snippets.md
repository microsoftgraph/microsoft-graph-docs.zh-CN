---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a11cd01f98873f3fa2207e487a340eecd3b20086a1aca9a38fd4f9efd6683760
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279409"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/applications/{id}/extensionProperties/{id}')
    .delete();

```
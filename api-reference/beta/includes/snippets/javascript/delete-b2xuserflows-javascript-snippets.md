---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a9a21a579946907fa5375cb74199aecb0a55b3fb3abce10f66a5327afc56945
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903461"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/b2xUserFlows/{id}')
    .version('beta')
    .delete();

```
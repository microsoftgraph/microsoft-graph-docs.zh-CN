---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc9bf45a059349740d9e52a871d3d4955f36919bdc935478b8388991686bd1a4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215842"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/apiConnectors/{id}')
    .version('beta')
    .delete();

```
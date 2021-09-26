---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6747dd060c4d88c5230f21896c6028c1feec11a9820a4b87b824564d99ccf56b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164171"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schemaExtension = await client.api('/schemaExtensions/graphlearn_test')
    .version('beta')
    .get();

```
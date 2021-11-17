---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e5d588f22d91236e9f76a391026b076d53db1a215d3503bc5276d61f32dcf21
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162188"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/onenote/pages/{id}')
    .version('beta')
    .delete();

```
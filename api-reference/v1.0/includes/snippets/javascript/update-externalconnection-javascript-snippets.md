---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6a975ff258e0435393b3e95a2743b7ab7c1594f
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53579953"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalConnection = {
  name: 'Contoso HR Service Tickets',
  description: 'Connection to index HR service tickets'
};

await client.api('/connections/contosohr')
    .update(externalConnection);

```
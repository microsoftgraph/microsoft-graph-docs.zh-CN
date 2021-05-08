---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f26d31cd970d2f782fec16513808d55c18a9d188
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241411"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let entries = await client.api('/admin/windows/updates/catalog/entries')
    .version('beta')
    .get();

```
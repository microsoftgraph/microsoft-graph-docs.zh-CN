---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b06af1b327bb5b551f65c9eb029a92c8a8029a9b
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332369"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/places/bldg1@contoso.com')
    .get();

```
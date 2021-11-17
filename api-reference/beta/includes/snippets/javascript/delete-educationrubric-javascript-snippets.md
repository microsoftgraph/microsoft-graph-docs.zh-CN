---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da731fb18682725cfcb8d2381e71999dc86e09003bf26cb366ed5300c6c54125
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162091"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/me/rubrics/{id}')
    .version('beta')
    .delete();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d921369e7a3570a47ca0107ec938b48be0a9bc626b6704c8dd2d1506cf035e46
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274335"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printServiceEndpoint = await client.api('/print/services/{id}/endpoints/{name}')
    .version('beta')
    .get();

```
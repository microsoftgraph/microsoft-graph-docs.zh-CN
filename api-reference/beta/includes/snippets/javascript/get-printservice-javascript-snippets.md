---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dbbe36dfe572dc972ba2928162223279d9cdc829492c85f9068d7ad39d552be0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329005"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printService = await client.api('/print/services/{id}')
    .version('beta')
    .get();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4165ee29167a911ce603fce48a1e3c5daddd0ad1e77b9c92b882b345edd2bdaf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903308"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let myRequests = await client.api('/privilegedApproval/myRequests')
    .version('beta')
    .get();

```
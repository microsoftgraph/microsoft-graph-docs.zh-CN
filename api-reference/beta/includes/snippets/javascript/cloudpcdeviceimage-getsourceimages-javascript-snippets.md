---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: edd54e169c38bdc5cdeb7dd1d5e6c3ce7f0c7a0d495953cd0d65a6e85b3caf79
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57331988"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getSourceImages = await client.api('/deviceManagement/virtualEndpoint/deviceImages/getSourceImages')
    .version('beta')
    .get();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3583fa1549281204efad1db8c40abd10a24ec6191ec0061e47e2363d0663d807
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333061"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let deployments = await client.api('/admin/windows/updates/deployments')
    .version('beta')
    .get();

```
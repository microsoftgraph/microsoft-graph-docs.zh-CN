---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e927feb5531cfcdf354fcd8aa4a57210b95694387f7f08a672cbfe777d6a055
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278289"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryObject = await client.api('/contacts/{id}/manager')
    .version('beta')
    .get();

```
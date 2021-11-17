---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26396868393efd315c9528773ac95e6ffc3513defe2dfb532f1fd0bb5c81e931
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903615"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tokenIssuancePolicies = await client.api('/policies/tokenIssuancePolicies')
    .version('beta')
    .get();

```
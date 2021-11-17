---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af6cc995cc391dade9cd5fcf39be58967169dba9354f52584610f6c2c3eff2ca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903955"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let place = await client.api('/places/bldg1@contoso.com')
    .version('beta')
    .get();

```
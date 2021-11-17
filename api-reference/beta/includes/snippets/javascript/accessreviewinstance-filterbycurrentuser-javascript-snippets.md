---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 463e5039a5f2d764ebaa90daa117d7a128574e591e15e97ae49d882e3f932cea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104146"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/identityGovernance/accessReviews/definitions/08531375-eff6-4e21-b1a8-de0eb37ec913/instances/filterByCurrentUser(on='reviewer')')
    .version('beta')
    .get();

```
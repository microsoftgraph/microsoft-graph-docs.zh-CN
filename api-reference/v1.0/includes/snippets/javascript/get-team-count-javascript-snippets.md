---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 67ac65d3dd1bd6e5539e711eb66ee7ef156ab8ba71f05e18b7c13c47bd27275d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903232"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let servicePrincipals = await client.api('/servicePrincipals')
    .header('ConsistencyLevel','eventual')
    .search('displayName:Team')
    .get();

```
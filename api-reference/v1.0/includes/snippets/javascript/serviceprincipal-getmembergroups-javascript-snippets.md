---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ba45799ef1c1dfe23ff16d9700f350aeb129b74eb0083d687495b8e118613c8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162371"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: true
};

await client.api('/servicePrincipals/{id}/getMemberGroups')
    .post(string);

```
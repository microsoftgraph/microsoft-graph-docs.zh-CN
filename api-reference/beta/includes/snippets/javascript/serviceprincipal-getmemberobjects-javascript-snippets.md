---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f07148c1363272a707432f8cd27e8b7e76ea6ab82c2e0169ed2fdd113e0b8dc8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903056"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: true
};

await client.api('/servicePrincipals/{id}/getMemberObjects')
    .version('beta')
    .post(string);

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60a040a67992a9394b5f53a77c195d7777bfd635b5f23e094e513010356e52ce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274408"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const forceDelete = {
  disableUserAccounts: true
};

await client.api('/domains/contoso.com/forceDelete')
    .version('beta')
    .post(forceDelete);

```
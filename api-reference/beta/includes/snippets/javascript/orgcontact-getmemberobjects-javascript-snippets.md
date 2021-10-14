---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c3d110fa43fab9128782925147fa0883c751dac24e7d0722fac4a853649070e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274352"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: true
};

await client.api('/contacts/{id}/getMemberObjects')
    .version('beta')
    .post(string);

```
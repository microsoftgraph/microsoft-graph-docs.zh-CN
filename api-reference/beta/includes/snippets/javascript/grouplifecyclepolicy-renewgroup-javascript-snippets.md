---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 11ea9b2f540e573e3bd563e673590643ddac2f28737bcbcd8bbff4a38dcf78fc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220676"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _boolean = {
  groupId: 'ffffffff-ffff-ffff-ffff-ffffffffffff'
};

await client.api('/groupLifecyclePolicies/renewGroup')
    .version('beta')
    .post(_boolean);

```
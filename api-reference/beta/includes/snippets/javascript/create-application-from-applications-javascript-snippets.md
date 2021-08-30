---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 329a2ae74eada8c34aa397802b79df661d90e8c3d932bf9c205ef4956bacd0c1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158562"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const application = {
  displayName: 'Display name'
};

await client.api('/applications')
    .version('beta')
    .post(application);

```
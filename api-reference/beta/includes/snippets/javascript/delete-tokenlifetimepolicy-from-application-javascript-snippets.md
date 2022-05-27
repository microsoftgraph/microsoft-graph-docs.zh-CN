---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cff5b43d861ee17be777ad72bd948dae74fd0ea8fcc2509e109e3cc5e781784a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158572"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/applications/{id}/tokenLifetimePolicies/{id}/$ref')
    .version('beta')
    .delete();

```
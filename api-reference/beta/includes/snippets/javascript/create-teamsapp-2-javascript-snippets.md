---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 100f3ba306ca2e08f43da62bbc335ae2bb5ab1cdff97cfc1a7e24561f41c4d2a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333709"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/appCatalogs/teamsApps?requiresReview=true')
    .version('beta')
    .post();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ed80d9824b883a640276af6ba3f8a5b1c344785
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690354"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/appCatalogs/teamsApps')
    .filter('externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'')
    .get();

```
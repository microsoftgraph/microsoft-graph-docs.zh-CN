---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f144a16e4ee2fa167939e80cdc9576c721183238
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50465235"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/appCatalogs/teamsApps')
    .filter('externalId eq \'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee\'')
    .get();

```
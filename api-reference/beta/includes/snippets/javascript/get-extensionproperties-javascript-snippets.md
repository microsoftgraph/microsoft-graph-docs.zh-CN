---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3205d7346200e25e95760da5b9687d43d77fd7d3f382d5e55d9db00275e88cf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215666"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let extensionProperties = await client.api('/applications/{id}/extensionProperties')
    .version('beta')
    .get();

```
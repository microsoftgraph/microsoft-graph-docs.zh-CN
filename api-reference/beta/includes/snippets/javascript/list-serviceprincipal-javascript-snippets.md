---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f26b05dca457d3a750a86ee7651869b483a07865743d2736391b11d81d707d57
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904014"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let servicePrincipals = await client.api('/servicePrincipals')
    .version('beta')
    .get();

```
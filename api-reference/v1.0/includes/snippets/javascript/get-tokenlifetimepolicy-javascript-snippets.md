---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9232296b0efd1bd529ea7bc89804c9fdbed7a4a1f94f0113120ebd4dd87a4e26
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903478"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tokenLifetimePolicy = await client.api('/policies/tokenLifetimePolicies/{id}')
    .get();

```
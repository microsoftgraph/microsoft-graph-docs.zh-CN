---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37086f5d128a38cba2bf1709ffd841e39a9869666d1e07a3643ff9dd9319dbca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409532"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let availableProviderTypes = await client.api('/identity/identityProviders/availableProviderTypes')
    .get();

```
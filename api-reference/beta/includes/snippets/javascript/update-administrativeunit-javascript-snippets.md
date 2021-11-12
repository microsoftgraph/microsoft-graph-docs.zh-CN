---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 983c7344e4a1b4dc3f5946a512e4fac78a4dcb70baff6cdd12e107bc3043d4fa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902552"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const administrativeUnit = {
  displayName: 'displayName-value',
  description: 'description-value',
  visibility: 'visibility-value'
};

await client.api('/administrativeUnits/{id}')
    .version('beta')
    .update(administrativeUnit);

```
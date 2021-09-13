---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d89143d21263932df44003bd635a83076303fcbad50dac59f2cd5d1198bb703d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277262"
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

await client.api('/directory/administrativeUnits/{id}')
    .update(administrativeUnit);

```
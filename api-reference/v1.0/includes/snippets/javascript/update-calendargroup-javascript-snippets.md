---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18d18dc081d2d9d82ac98ee9733a97e7ada23e149a5eb62adb1e362e37ac0632
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277566"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendarGroup = {
  name: 'name-value'
};

await client.api('/me/calendarGroups/{id}')
    .update(calendarGroup);

```
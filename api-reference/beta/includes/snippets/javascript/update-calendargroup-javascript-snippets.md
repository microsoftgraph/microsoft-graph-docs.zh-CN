---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00ae9b5bef1de1208b593df35616b4beae28262c989b2716d3820ae264221d98
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218614"
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
    .version('beta')
    .update(calendarGroup);

```
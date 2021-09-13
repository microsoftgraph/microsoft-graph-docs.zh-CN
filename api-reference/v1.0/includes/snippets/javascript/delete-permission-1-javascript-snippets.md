---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5fc106529c6db566f489e1e08d16ca507448d8ed4859e65211bbb4c0330863d5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104312"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{item-id}/permissions/{perm-id}')
    .delete();

```
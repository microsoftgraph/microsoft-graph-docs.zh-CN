---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f3dbdb56a6f61f93c146ee7640acf483040fb39
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223285"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directory/administrativeUnits/{id}')
    .delete();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e2c009183c0991da1045024c9864be860e711ad
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801282"
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
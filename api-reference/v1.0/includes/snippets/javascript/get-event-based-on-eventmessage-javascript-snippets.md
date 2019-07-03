---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b052104f89e0ab0f8f601fa685f2c4592bd5d12a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466796"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkADYAAAImV_jAAA=')
    .expand('eventMessage/event')
    .get();

```
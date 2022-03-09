---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 05d405a6563f30566a335761a53dc804d4278e32
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60684091"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connectionOperation = await client.api('/external/connections/contosohr/operations/3ed1595a-4bae-43c2-acda-ef973e581323')
    .get();

```
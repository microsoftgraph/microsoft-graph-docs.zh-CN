---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 053dbc3d75efb488a94e97a977809ba44bb93095
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696152"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let externalConnection = await client.api('/external/connections/contosohr')
    .version('beta')
    .get();

```
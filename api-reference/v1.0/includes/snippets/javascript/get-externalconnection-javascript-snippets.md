---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 844a78985e5d393e353e0ad37fcb0a56e5c439c6
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694797"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let externalConnection = await client.api('/external/connections/contosohr')
    .get();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ebf9a83d435ab2146ce78e4f6cefa9488fb215a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612706"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedRoleAssignmentRequests')
    .version('beta')
    .get();

```
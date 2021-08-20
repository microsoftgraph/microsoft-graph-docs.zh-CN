---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f9bc0fc5621a797b3b0bd86839d8303d95140b2032c6a6a984f6c29de9f1546
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218790"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationAssignmentSettings = await client.api('/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentSettings')
    .get();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 416526ad83157fee2fb37191c594de4512f53af1
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142241"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications/{id}/tokenIssuancePolicies')
    .version('beta')
    .get();

```
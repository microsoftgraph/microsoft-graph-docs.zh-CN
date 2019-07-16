---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 11d39ab73dd03bc3e09f73de02869b326ef9d4c5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739477"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365ActivationsUserDetail')
    .get();

```
---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dcbb978c2ed2a22f9b7c9dd15fea3c7562b3ef27
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35727304"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOneDriveActivityUserDetail(period='D7')')
    .version('beta')
    .get();

```
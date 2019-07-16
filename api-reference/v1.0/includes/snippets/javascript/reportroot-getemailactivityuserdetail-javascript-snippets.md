---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 44e4c2978e315b03a05e01ab555079fbb0e5eeca
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737574"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getEmailActivityUserDetail(period='D7')')
    .get();

```
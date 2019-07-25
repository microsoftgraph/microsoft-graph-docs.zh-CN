---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7f0ada3bf867bca0cb81d591ccc622a314355c46
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35727091"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointActivityPages(period='D7')')
    .version('beta')
    .get();

```
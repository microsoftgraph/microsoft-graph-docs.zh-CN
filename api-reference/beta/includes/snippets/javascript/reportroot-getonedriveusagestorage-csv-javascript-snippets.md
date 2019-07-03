---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 54ba0d5865ed42cc38d01d75e3b695a6f71ce0af
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477935"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOneDriveUsageStorage(period='D7')')
    .version('beta')
    .get();

```
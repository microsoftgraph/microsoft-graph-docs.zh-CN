---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 29bfcc869bb8e510c4c511ad2dee73f00fd6f4d2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500632"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const agreement = {
  displayName: "displayName-value",
  isViewingBeforeAcceptanceRequired: true
};

let res = await client.api('/agreements/'id'')
    .version('beta')
    .update({agreement : agreement});

```
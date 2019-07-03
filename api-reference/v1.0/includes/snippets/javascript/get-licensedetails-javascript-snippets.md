---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f0b0c9bfb6d49b5220be52a6f3b394cc97bd99be
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466826"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/licenseDetails')
    .get();

```
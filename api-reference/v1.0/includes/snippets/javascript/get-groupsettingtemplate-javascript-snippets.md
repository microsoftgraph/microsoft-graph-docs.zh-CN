---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 69690db4ebfede451cf09b69f0582d4910d8129d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467675"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groupSettingTemplates/{id}')
    .get();

```
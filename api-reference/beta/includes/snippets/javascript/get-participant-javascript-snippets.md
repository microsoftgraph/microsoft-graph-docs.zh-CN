---
description: 自动生成的文件。 不修改
ms.openlocfilehash: af591176597740220c211b93ad098551bc6d7a5e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479901"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/app/calls/{id}/participants/{id}')
    .version('beta')
    .get();

```
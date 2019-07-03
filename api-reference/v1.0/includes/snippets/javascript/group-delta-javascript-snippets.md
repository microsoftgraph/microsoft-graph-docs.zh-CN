---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ef3038091c30f73f7063b8656faf65d8bda3a167
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493154"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/delta')
    .header('Prefer','return=minimal')
    .select('displayName,description,mailNickname')
    .get();

```
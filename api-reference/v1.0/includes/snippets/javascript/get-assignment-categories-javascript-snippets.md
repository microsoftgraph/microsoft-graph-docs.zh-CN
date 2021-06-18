---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92cd6a99faaa085b518a1c7d5f897a846e21ef17
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991076"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let categories = await client.api('/education/classes/a17025d0-62a8-4450-9e6e-db31d8c8feb8/assignments/1fdf61ee-c129-4960-9b7c-8df159aa64b0/categories')
    .get();

```
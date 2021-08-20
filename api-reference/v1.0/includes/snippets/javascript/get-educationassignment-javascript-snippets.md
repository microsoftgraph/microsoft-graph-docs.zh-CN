---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76bba3a25c000d4dd1cb662e943975d67de2a98fade0d433dc7da04eeb3a7e8e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277180"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationAssignment = await client.api('/education/classes/5edb6a5f-fc6b-441b-8952-bcbfc33ef0e5/assignments/1fdf61ee-c129-4960-9b7c-8df159aa64b0')
    .get();

```
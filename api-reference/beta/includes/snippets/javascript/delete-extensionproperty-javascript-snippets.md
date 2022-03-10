---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1191fa79c498aa390b5f510f6c057a1743206284
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412374"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/applications/fd918e4b-c821-4efb-b50a-5eddd23afc6f/extensionProperties/')
    .version('beta')
    .delete();

```
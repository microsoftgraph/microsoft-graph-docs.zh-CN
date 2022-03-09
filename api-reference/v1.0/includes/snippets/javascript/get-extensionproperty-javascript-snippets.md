---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56dd72bd15bcf3d7fe8db5255f169a9f5d0eff02
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394283"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let extensionProperty = await client.api('/applications/fd918e4b-c821-4efb-b50a-5eddd23afc6f/extensionProperties/1f0f15e3-925d-40f0-8fc8-9d3ad135bce0')
    .get();

```
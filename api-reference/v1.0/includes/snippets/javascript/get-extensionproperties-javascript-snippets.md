---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0f2dbc2c663a6906a276a84c6483b57f3db3983
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412406"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let extensionProperties = await client.api('/applications/fd918e4b-c821-4efb-b50a-5eddd23afc6f/extensionProperties')
    .get();

```
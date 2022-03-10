---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08853a5eab739ba941426c31b6a025f21d8a894b
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411632"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/applications/fd918e4b-c821-4efb-b50a-5eddd23afc6f/extensionProperties/')
    .delete();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7a65c7453907e3126fb07600289693193a19931
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63351190"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let profile = await client.api('/me/profile')
    .version('beta')
    .expand('names($select=first,last),skills($select=displayName)')
    .get();

```
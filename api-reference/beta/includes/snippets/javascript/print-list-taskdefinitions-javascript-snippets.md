---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41a2d8353a559c1d6b52168244d8e0217d329bd7760519f6c4ae89e449e0b3a1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279037"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let taskDefinitions = await client.api('/print/taskDefinitions')
    .version('beta')
    .get();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c55389bacd83fa2d3a9e997afdce5f3cf5b3f0c0a6edc7c48219b4bc39169cd5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164316"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let positions = await client.api('/me/profile/positions')
    .version('beta')
    .get();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 107a9938968254cad9b641b6f4cf73ac1ac3fc83
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629283"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getSubscriptions = await client.api('/deviceManagement/virtualEndpoint/snapshots/getSubscriptions')
    .version('beta')
    .get();

```
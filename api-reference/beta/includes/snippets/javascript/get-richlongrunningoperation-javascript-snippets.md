---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0266f4092d29383e0812e7ba93507abff2706b07
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225829"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let richLongRunningOperation = await client.api('/sites/{siteId}/operations/{richLongRunningOperation-ID}')
    .version('beta')
    .get();

```
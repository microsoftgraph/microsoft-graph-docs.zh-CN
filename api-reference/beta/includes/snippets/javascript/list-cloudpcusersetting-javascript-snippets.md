---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13311a719dd50ac3510ef2c0875976011e3d71e5
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208382"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userSettings = await client.api('/deviceManagement/virtualEndpoint/userSettings')
    .version('beta')
    .get();

```
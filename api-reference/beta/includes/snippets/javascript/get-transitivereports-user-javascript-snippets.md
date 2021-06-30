---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c1eb267c20aacfd69d96d767e44f7f5c05f282d
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210827"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let int32 = await client.api('/users/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4/transitiveReports/$count')
    .version('beta')
    .get();

```
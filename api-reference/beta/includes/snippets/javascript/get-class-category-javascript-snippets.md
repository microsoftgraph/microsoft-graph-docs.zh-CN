---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a983740f2cabd3c71bc7c5ed0b41c6f24edefbe
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991686"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationCategory = await client.api('/education/classes/dacbf757-888d-42ae-b701-5e57cec300ae/assignmentCategories/7f64924d-4cdb-4e54-8c37-c0f3d46f0747')
    .version('beta')
    .get();

```
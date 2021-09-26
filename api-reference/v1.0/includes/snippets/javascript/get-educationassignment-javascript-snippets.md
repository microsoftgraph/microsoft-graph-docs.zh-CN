---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b56cb5225fede78f52ca5882d229387a6a8406e
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59765932"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationAssignment = await client.api('/education/classes/f4a941ff-9da6-4707-ba5b-0eae93cad0b4/assignments/3c77de7f-539b-49e1-9c96-1274f2f0ee3b')
    .get();

```
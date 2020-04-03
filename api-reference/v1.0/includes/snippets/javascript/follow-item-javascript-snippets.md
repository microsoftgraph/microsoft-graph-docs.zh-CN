---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a523c7279c3f965ef7221b4251a06bfe227c95b
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124398"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/follow')
    .post();

```
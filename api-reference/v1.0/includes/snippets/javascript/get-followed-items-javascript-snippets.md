---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0ddbfb3dfd9f37ded00405e04ccd8ec42aee6f0
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124348"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/following')
    .get();

```
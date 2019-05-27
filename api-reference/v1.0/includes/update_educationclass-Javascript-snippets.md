---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 76a1d2c781cdc3d20f1f34c3d5f512f21c5b8c10
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463254"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationClass = {
  description: "History - World History 1",
  displayName: "World History Level 1",
};

let res = await client.api('/education/classes/{class-id}')
    .update({educationClass : educationClass});

```
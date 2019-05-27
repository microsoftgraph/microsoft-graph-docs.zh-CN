---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ad6acf858672c7db56715ad8d3224b6ae4da1f57
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34470224"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationClass = {
 @odata.id:"https://graph.microsoft.com/v1.0/education/classes/11006"
};

let res = await client.api('/education/schools/{school-id}/classes/$ref')
    .post({educationClass : educationClass});

```
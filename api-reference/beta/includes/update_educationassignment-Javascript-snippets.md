---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bea1f1e49952334bc8b2e6cdbe3c31b535ddcfcc
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461289"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationAssignment = {
  displayName: "Week 1 reading assignment",
  instructions: {
    contentType: "Text",
    content: "Read chapters 1 through 3"
  },
  dueDateTime: "2014-02-01T00:00:00Z"
};

let res = await client.api('/education/classes/11021/assignments/19002')
    .version('beta')
    .update({educationAssignment : educationAssignment});

```
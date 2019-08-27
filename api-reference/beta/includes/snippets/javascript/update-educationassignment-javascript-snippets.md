---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 88b9a645374634f76a6390f542fb0ee4a2804bb1
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636525"
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
    .update(educationAssignment);

```
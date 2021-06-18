---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 841f85c0caeca40f8a196598121c8b2d78969cd0
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993551"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationAssignment = {
  displayName: 'Week 1 reading assignment',
  instructions: {
    contentType: 'Text',
    content: 'Read chapters 1 through 3'
  },
  dueDateTime: '2014-02-01T00:00:00Z'
};

await client.api('/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8')
    .update(educationAssignment);

```
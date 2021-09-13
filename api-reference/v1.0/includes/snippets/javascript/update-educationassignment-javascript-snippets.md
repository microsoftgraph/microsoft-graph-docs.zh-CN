---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 529e9329f6e2a235d97b840b42ce18276d104fa5034e6b25663b3aa27898f9b8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105404"
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
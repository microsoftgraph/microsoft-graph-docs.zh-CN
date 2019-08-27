---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1f8877c280de88ba2fe5722714fd6329c2e112a3
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636522"
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

let res = await client.api('/education/classes/11014')
    .version('beta')
    .update(educationClass);

```
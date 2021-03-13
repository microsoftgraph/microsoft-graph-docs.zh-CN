---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8977dd4c22915b8a7a8e1164e72fc29c01872a7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808641"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationClass = {
  description: 'History - World History 1',
  displayName: 'World History Level 1',
};

await client.api('/education/classes/11014')
    .version('beta')
    .update(educationClass);

```
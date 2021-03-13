---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc9bdd8d6883af241cfae3627025d51ada6d1ea3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793508"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let extensionProperties = await client.api('/applications/{id}/extensionProperties')
    .version('beta')
    .get();

```
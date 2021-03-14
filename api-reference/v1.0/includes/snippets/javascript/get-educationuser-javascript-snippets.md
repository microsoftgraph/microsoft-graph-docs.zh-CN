---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c7052f801bc84da364b906583fce7a93629ef4e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784029"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let user = await client.api('/education/me/user')
    .get();

```
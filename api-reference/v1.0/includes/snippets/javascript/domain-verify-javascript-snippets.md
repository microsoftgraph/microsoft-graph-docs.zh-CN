---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3320e22e4ca9f9604545b1e0eb6e37af2228101e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791524"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/domains/{domain-name}/verify')
    .post();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe9c1636bf1805479f279f67eda411c4b9dac144
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794141"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bundles = await client.api('/drive/bundles')
    .version('beta')
    .get();

```
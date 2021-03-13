---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63495fa1f72f2b248be80050d0b77b7758545a3c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790384"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let message = await client.api('/me/messages/AAMkAGE1M2_bs88AACHsLqWAAA=/')
    .version('beta')
    .expand('singleValueExtendedProperties($filter=id%20eq%20\'String%20%7B66f5a359-4659-4830-9070-00047ec6ac6e%7D%20Name%20Color\')')
    .get();

```
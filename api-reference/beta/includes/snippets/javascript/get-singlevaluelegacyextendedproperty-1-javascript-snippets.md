---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6aceb88a2195d3d2055353bebd9d419d7cb394da
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50465367"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkAGE1M2_bs88AACHsLqWAAA=/')
    .version('beta')
    .expand('singleValueExtendedProperties($filter=id%20eq%20\'String%20%7B66f5a359-4659-4830-9070-00047ec6ac6e%7D%20Name%20Color\')')
    .get();

```
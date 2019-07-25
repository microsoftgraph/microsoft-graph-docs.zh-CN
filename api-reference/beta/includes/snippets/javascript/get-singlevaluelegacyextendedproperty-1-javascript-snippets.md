---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 646445391bc06cf2dca8a1b041c4a226bb2ac2a3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717568"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkAGE1M2_bs88AACHsLqWAAA=/')
    .version('beta')
    .filter('id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color')')
    .expand('singleValueExtendedProperties($filter=id%20eq%20'String%20%7B66f5a359-4659-4830-9070-00047ec6ac6e%7D%20Name%20Color')')
    .get();

```
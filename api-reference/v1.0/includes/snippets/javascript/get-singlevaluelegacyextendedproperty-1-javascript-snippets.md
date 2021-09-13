---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b2d5997f91dbf49ccbe8dac24ced45df46e4db2b4ba11307af20bf0e0cd932b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333345"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let message = await client.api('/me/messages/AAMkAGE1M2_bs88AACHsLqWAAA=')
    .expand('singleValueExtendedProperties($filter=id%20eq%20\'String%20%7B66f5a359-4659-4830-9070-00047ec6ac6e%7D%20Name%20Color\')')
    .get();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41554d5f9f053efbd15328cb50a980382e3e8bdb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797909"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bundles = await client.api('/drive/bundles?filter=bundle/album%20ne%20null')
    .version('beta')
    .filter('bundle/album ne null')
    .get();

```
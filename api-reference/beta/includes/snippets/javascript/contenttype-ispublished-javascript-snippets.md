---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75ccfbb9da21e24a25d7b608bc72adff0ab78a40
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770569"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let _boolean = await client.api('/sites/{siteId}/contentTypes/{contentTypeId}/isPublished')
    .version('beta')
    .get();

```
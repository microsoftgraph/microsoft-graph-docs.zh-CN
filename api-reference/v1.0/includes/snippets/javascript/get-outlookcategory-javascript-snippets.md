---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 836ba41be248a0ee031020f4c84041d039373fc2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785564"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let outlookCategory = await client.api('/me/outlook/masterCategories/de912e4d-c790-4da9-949c-ccd933aaa0f7')
    .get();

```
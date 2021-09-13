---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c99d6396814d4b63fee1195a9bf5e20325cff981
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59062984"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let columns = await client.api('/sites/{site-id}/lists/{list-id}/columns')
    .get();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6be237a65480512fa15965141471f23b206a1019
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59080197"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}')
    .delete();

```
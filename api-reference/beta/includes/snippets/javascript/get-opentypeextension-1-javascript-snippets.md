---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54cf266007b8d3e86b20753b06351e2758187622
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605130"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==='/extensions/Com.Contoso.Referral')
    .version('beta')
    .get();

```
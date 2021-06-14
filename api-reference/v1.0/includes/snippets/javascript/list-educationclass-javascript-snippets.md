---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd9be76d955ab04c6094cbe706b1dd9382fb4b91
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52871600"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let taughtClasses = await client.api('/education/users/{educationUserId}/taughtClasses')
    .get();

```
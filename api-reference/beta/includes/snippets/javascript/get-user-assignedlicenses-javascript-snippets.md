---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 736b39a90636ceed15c822f662575d3b445ddf7e
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59765053"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let users = await client.api('/users')
    .version('beta')
    .filter('assignedLicenses/any(u:u/skuId eq cbdc14ab-d96c-4c30-b9f4-6ada7cdc1d46)')
    .select('id,mail,assignedLicenses')
    .get();

```
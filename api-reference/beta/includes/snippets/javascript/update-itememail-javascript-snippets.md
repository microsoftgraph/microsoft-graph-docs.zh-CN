---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 87a262586f5edf38094e7a1f7149666f737485d3
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37997353"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemEmail = {
  address: "address-value",
  displayName: "displayName-value",
  type: "type-value"
};

let res = await client.api('/me/profile/emails/{id}')
    .version('beta')
    .update(itemEmail);

```
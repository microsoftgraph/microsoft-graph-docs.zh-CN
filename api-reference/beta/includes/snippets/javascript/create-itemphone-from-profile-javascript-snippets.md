---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c55a61877cd7e1c613e4fa57adb5b0f53639a39
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996526"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemPhone = {
  displayName: "displayName-value",
  type: "type-value",
  number: "number-value"
};

let res = await client.api('/me/profile/phones')
    .version('beta')
    .post(itemPhone);

```
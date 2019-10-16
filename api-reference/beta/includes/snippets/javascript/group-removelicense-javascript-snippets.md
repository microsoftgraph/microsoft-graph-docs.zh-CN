---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 288d651e689be37b7140d1c6a6c5a6f1bf390d1b
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535583"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  addLicenses: [],
  removeLicenses: ["skuId-value-1", "skuId-value-2"]
};

let res = await client.api('/groups/1ad75eeb-7e5a-4367-a493-9214d90d54d0/assignLicense')
    .version('beta')
    .post(group);

```
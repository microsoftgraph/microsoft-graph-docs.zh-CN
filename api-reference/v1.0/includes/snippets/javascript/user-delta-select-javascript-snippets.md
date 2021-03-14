---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58158e376af81018f47a03f4c47c9331480b408a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780431"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/users/delta')
    .select('displayName,jobTitle,mobilePhone')
    .get();

```
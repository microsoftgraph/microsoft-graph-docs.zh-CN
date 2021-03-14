---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 156a0785278127620ae48d8a099b861fc47698a7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778857"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let licenseDetails = await client.api('/me/licenseDetails')
    .get();

```
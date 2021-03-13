---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6578fbe740e723a385ca867281a017f4cf05e1f3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808278"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/047dd774-f1c4-40f2-82f0-278de79f9b83/reprocessLicenseAssignment')
    .version('beta')
    .post();

```
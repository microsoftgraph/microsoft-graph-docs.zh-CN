---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ada8dd1125f5fa2d93985e9c923a20f1d4bb9d71
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787833"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/047dd774-f1c4-40f2-82f0-278de79f9b83/reprocessLicenseAssignment')
    .post();

```
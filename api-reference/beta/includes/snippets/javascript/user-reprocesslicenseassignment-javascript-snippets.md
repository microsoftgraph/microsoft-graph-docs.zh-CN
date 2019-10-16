---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50d4981abaad160d49fb735f0e8f4a7b30a58dd1
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538395"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/047dd774-f1c4-40f2-82f0-278de79f9b83/reprocessLicenseAssignment')
    .version('beta')
    .post();

```
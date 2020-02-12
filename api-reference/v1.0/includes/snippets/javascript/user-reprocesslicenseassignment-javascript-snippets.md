---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70c6bc228c808b31a4b3c2834666f0ccdaa2a529
ms.sourcegitcommit: 1a84f80798692fc0381b1acecfe023b3ce6ab02c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2020
ms.locfileid: "41953631"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/047dd774-f1c4-40f2-82f0-278de79f9b83/reprocessLicenseAssignment')
    .post();

```
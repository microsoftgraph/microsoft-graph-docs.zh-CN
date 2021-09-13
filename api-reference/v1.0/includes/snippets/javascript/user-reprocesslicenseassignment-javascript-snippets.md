---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6b4492e8e8dd80375273a1c78a685f72a37cb2a99af16669a893ff297ed60c4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219085"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/047dd774-f1c4-40f2-82f0-278de79f9b83/reprocessLicenseAssignment')
    .post();

```
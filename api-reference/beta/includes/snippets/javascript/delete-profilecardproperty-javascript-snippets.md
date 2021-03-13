---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66ae95ff450f2c6c5ddbeee4fe0e0f9f1732e434
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780538"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/organization/{organizationId}/settings/profileCardProperties/fax')
    .version('beta')
    .delete();

```
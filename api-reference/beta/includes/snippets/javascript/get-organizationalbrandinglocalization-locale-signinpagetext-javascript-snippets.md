---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b187abd40d360529e2ac1cba2ea0e861ea158245
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996823"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let string = await client.api('/organization/99b24e1b-abec-4598-9d63-a2baf0a3cea1/branding/localizations/fr-FR/signInPageText')
    .version('beta')
    .get();

```
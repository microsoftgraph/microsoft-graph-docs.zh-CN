---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04ede3e61b7679f1d9f5d179d4949597f8c9f00f
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62224735"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userRegistrationDetails = await client.api('/reports/authenticationMethods/userRegistrationDetails')
    .version('beta')
    .get();

```
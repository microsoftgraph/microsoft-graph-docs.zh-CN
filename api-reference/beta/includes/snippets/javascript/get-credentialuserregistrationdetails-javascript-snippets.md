---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 337567d259a8a6335ed6dcdc26ce918d8561c7b9a6f4f4df279868ca0a31107a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164145"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let credentialUserRegistrationDetails = await client.api('/reports/credentialUserRegistrationDetails')
    .version('beta')
    .get();

```
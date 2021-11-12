---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1eae52ec2cd78464e70e737ed6d2478b65592c45d927f57f8e3574f7d0c883ad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279242"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let licenseDetails = await client.api('/me/licenseDetails')
    .version('beta')
    .get();

```
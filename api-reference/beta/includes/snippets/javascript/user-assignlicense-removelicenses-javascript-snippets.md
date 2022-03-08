---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6df2dc086c1ce0ba2bd68ab1150ff23557e0b139
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63340020"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
    addLicenses: [],
    removeLicenses: [
        'f30db892-07e9-47e9-837c-80727f46fd3d',
        '84a661c4-e949-4bd2-a560-ed7766fcaf2b'
    ]
};

await client.api('/me/assignLicense')
    .version('beta')
    .post(user);

```
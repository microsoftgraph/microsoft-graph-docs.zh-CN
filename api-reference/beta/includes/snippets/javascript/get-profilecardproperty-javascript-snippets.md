---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eee6fb649c3404f75c541e2e749e1ab24b146936
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080759"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/organization/settings/profileCardProperties/{id}')
    .version('beta')
    .get();

```
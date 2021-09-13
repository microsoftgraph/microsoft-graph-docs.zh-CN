---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 608b822025c1808b8382ab3f84551571306f03e734a13f57e050061cc1cdda56
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164086"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let personCertification = await client.api('/me/profile/certifications/{id}')
    .version('beta')
    .get();

```
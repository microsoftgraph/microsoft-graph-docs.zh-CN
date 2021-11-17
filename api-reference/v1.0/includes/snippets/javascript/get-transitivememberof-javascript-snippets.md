---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7d8060f9f193b72f468e485af2bf7bbb3342dd2b98085320a2a3097525f658d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106401"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let transitiveMemberOf = await client.api('/users/{id}/transitiveMemberOf')
    .get();

```
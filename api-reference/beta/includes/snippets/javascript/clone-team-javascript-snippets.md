---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7dd6e81944b07273ce56d71a2efb8e49705fbbd
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332462"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const clone = {
     displayName: "Library Assist",
     description: "Self help community for library",
     mailNickname: "libassist",
     partsToClone: "apps,tabs,settings,channels,members",
     visibility: "public"
};

let res = await client.api('/teams/{id}/clone')
    .version('beta')
    .post(clone);

```
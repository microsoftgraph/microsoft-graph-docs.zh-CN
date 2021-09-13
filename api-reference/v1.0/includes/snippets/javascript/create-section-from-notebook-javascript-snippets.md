---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71e13c8a2d61e99aa41d0474b941529ec4b89ed2de232e3f78bb4e9cd4d35d67
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215988"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteSection = {
  displayName: 'Section name'
};

await client.api('/me/onenote/notebooks/{id}/sections')
    .post(onenoteSection);

```
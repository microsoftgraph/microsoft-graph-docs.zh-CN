---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bbb35c9ea50854337609730a12bbc84d908df3dedb226266764256316c5ca500
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277803"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryRole = {
  roleTemplateId: 'fe930be7-5e62-47db-91af-98c3a49a38b1'
};

await client.api('/directoryRoles')
    .version('beta')
    .post(directoryRole);

```
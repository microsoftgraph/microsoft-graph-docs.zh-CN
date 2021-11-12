---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 11937e49f9c20dcd63ea7c404608c2012c0f000296bc6715fd3b813e373de314
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164201"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  '@odata.id':'https://graph.microsoft.com/beta/education/users/13015'
};

await client.api('/education/classes/11011/members/$ref')
    .version('beta')
    .post(educationUser);

```
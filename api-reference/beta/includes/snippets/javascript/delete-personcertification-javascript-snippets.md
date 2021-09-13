---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c2401b092cdcec65f282bfad1a55483809f13974f18dbdd8c4f9468e8bf3b0c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219127"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/{userId}/profile/certifications/{id}')
    .version('beta')
    .delete();

```
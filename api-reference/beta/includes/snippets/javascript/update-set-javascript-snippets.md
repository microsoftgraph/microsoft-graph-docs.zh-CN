---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 294bba6d7d004a02cbf8685ada9d5d1517302b00ee71911a37dda5417d2b93cc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277972"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const set = {
  description: 'mySet'
};

await client.api('/termStore/sets/{setId}')
    .version('beta')
    .update(set);

```
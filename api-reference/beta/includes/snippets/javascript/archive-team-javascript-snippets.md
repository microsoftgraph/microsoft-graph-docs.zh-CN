---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99c6a9148225f0eee9f580d7665d4ae50560cb455e607c2b37317be5628bddfa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332859"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{id}/archive')
    .version('beta')
    .post();

```
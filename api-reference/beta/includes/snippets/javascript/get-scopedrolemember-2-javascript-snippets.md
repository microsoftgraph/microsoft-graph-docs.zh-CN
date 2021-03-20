---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60cc29e140949ff21df897a55db6843cc27c4754
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942962"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let scopedRoleMembers = await client.api('/administrativeUnits/{id}/scopedRoleMembers')
    .version('beta')
    .get();

```
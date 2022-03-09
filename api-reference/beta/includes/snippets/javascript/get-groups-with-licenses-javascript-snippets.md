---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f276c9923fd0d761fe914a7139162b83ae1a942
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393387"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groups = await client.api('/groups')
    .version('beta')
    .filter('assignedLicenses/any()')
    .select('id,assignedLicenses')
    .get();

```
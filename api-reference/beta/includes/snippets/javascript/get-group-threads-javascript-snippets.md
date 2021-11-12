---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90e93c05703c69a994cab27b0b0898d8011e3e5cf319e6c55d7549794ac0986d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277784"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let threads = await client.api('/groups/{id}/threads')
    .version('beta')
    .get();

```
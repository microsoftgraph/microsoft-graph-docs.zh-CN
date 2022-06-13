---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb8f785251949e4530330ebb2efc8834fcde83e7
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66040870"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/directory/administrativeUnits/{id1}/members/{id2}/$ref')
    .delete();

```
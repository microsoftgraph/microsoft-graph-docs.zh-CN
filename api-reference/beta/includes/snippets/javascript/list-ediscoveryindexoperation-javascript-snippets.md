---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2064e3ededd76a085ee548e8bb33808dd60e01e0
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095999"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let ediscoveryIndexOperation = await client.api('/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/0053a61a3b6c42738f7606791716a22a/lastIndexOperation')
    .version('beta')
    .get();

```
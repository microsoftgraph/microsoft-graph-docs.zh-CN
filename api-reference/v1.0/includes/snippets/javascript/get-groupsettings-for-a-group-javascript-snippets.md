---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e05d9d80702499502e5d128e487fef879c9efa6
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63397286"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let settings = await client.api('/groups/05aa6a98-956a-45c0-b13b-88076a23f2cd/settings')
    .get();

```
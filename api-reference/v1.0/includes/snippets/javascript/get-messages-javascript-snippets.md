---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63f3001cfcd15c6589627ee4e21232cfd7f9308046b3210b0b57b925da709aa8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409304"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messages = await client.api('/me/messages')
    .select('sender,subject')
    .get();

```
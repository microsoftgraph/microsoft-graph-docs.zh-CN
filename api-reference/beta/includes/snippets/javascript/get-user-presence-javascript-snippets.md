---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a7c48c6f86e1567d09b0e8019ef023f1e18d8f6
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867685"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/66825e03-7ef5-42da-9069-724602c31f6b/presence')
    .version('beta')
    .get();

```
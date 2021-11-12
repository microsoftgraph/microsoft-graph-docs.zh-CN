---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5674ca248f001fe0f1666cf53db6e022a4fde82086446a4f6d8eb1d75cb6dcb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277785"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let rejectedSenders = await client.api('/groups/{id}/rejectedSenders')
    .version('beta')
    .get();

```
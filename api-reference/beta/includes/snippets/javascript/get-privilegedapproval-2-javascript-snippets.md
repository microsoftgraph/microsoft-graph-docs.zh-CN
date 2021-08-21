---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c09f87603ea88abcced2a3b8c273579186889e41726c87b68267e2ebd3a25b1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218462"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let privilegedApproval = await client.api('/privilegedApproval')
    .version('beta')
    .get();

```
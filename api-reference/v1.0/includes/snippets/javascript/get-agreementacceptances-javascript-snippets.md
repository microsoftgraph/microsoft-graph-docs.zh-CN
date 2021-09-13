---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e4650efb6b44585c62cec353b621a053110c4573c0a5a2155e2423133c6e82c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105081"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let agreementAcceptances = await client.api('/me/agreementAcceptances')
    .get();

```
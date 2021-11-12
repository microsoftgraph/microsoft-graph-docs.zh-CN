---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6de1630035090edf12adf6acb8d6e5d83e4d8a7627de545255bc71676d8f73b3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902374"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printerShare = await client.api('/print/shares/{id}')
    .version('beta')
    .get();

```
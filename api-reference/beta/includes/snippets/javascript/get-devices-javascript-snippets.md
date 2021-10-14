---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0723defe300cad3824a8ce6248c4c29e9dc076065c9780431a8846308767aea5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218949"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let devices = await client.api('/devices')
    .version('beta')
    .get();

```
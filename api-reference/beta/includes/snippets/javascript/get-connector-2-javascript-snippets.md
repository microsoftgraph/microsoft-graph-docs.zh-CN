---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9126fcd3b3c73dc6467b6c646217a1835ab1296e32397fa47d7824e0cb4785a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162184"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printConnector = await client.api('/print/connectors/{id}')
    .version('beta')
    .get();

```
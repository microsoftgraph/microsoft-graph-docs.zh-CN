---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18aaa4f36c2817fe7f760a9b3ccbd654fd9b201645603bc612f45f597f71367a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105216"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drive = await client.api('/users/{idOrUserPrincipalName}/drive')
    .version('beta')
    .get();

```
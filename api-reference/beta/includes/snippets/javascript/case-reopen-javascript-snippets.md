---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d55e409bd190c1bb9e883d249a7b5e4d4d72d7caf138c59bf8cbcff0f91933a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278791"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583/reopen')
    .version('beta')
    .post();

```
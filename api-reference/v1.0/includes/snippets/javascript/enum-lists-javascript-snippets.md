---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39e3f5997b48b26a002ef217e2cfce89037a3e438bf07b662ce4942f85c897e2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219335"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let lists = await client.api('/sites/{site-id}/lists')
    .get();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f8c7062f1fa923e21f268fc96e083683f7a213a228684982a6d62c1b7a7b716
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409357"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let driveItem = await client.api('/teams/{id}/channels/{id}/filesFolder')
    .get();

```
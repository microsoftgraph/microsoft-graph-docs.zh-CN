---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5bd0fb388903e2e35108d8b7b0b2ad7f60de52da68d9e03d650435d6d7f0544b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278486"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/conversations/{id}')
    .version('beta')
    .delete();

```
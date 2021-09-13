---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef5e50f6a96ec8ef7e56478d9d9dd2e89da944b64a1c492d3b9891e944d64f95
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903539"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/me/rubrics/ceb3863e-6912-4ea9-ac41-3c2bb7b6672d')
    .delete();

```
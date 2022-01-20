---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04411c0e5c7d3d6c11210a87250399ea0f34f36cbc095297cfa5b207368a6ff9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273977"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let supportedLanguages = await client.api('/me/outlook/supportedLanguages')
    .version('beta')
    .get();

```
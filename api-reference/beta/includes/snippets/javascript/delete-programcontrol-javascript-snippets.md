---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3119959624f8c791dd527d0bf63ed1c0dc0db416a1feff317ea00b969a9e04e4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279480"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/programControls/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
    .version('beta')
    .delete();

```
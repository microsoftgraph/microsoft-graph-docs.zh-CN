---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aec66e26860a5c70d1e7675c1fd1564c57be7ca9
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212234"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let incomingChannels = await client.api('/teams/893075dd-2487-4122-925f-022c42e20265/incomingChannels')
    .version('beta')
    .get();

```
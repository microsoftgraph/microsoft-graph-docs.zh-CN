---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9434b25362d54cb07e12df7daf47602aaa375103
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212563"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let allChannels = await client.api('/teams/893075dd-2487-4122-925f-022c42e20265/allChannels')
    .version('beta')
    .get();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc94823a9c9bade6af2f1f4866d69f955db1d08e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212529"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let allChannels = await client.api('/teams/893075dd-2487-4122-925f-022c42e20265/allChannels')
    .version('beta')
    .filter('membershipType eq \'shared\'')
    .get();

```
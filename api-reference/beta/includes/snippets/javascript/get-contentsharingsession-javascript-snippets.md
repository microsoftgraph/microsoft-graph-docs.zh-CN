---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34e5313df02772e58cb84c40e0e33532d2de16db
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210360"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contentSharingSession = await client.api('/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/contentSharingSessions/7e1b4346-85a6-4bdd-abe3-d11c5d420efe')
    .version('beta')
    .get();

```
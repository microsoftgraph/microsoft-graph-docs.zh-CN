---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a5e6b713654982fa41402c4de88e784f6e92ad5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964388"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tabs = await client.api('/teams/6903fa93-605b-43ef-920e-77c4729f8258/channels/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/tabs')
    .expand('teamsApp')
    .get();

```
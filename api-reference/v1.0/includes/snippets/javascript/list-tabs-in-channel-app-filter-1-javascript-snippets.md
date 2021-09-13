---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7cadb5967a65468c3e979cc7e80bf411ebce26060c430a331b70c94f04d2bfba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277557"
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
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: efc2eecdd5b5261933c39228319b2f314a9a658fc86350f778012ad433cab003
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163015"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drives = await client.api('/groups/{groupId}/drives')
    .get();

```
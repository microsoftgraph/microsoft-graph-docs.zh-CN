---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4c42525f78cdcfede9a8963601ceaf037fdff2dd2f151cc5ebec79649cf4ee5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903576"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id':'https://graph.microsoft.com/v1.0/groups/{id}'
};

await client.api('/directory/administrativeUnits/{id}/members/$ref')
    .post(directoryObject);

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2edb59755b8b6ee6e8918cd815245bc19a759878
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202137"
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
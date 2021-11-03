---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8540ee0ed46e3536900888b7a23ece3564481f34
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687802"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalGroup = {
  displayName: 'Contoso Marketing',
  description: 'The product marketing team'
};

await client.api('/external/connections/{connectionsId}/groups/{externalGroupId}')
    .update(externalGroup);

```
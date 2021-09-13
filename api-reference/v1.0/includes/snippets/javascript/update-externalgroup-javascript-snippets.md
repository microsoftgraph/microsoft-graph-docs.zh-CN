---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 503bfdfb5bb74c1bc83edfed64eb0b0d787f099e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022371"
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

await client.api('/connections/{connectionsId}/groups/{externalGroupId}')
    .update(externalGroup);

```
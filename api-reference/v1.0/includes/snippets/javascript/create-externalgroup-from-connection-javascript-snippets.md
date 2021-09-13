---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94a153ce381c1b134bc4021a9d3f3d901d1a6e0d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022495"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalGroup = {
  id: '31bea3d537902000',
  displayName: 'Contoso Marketing',
  description: 'The product marketing team'
};

await client.api('/external/connections/contosohr/groups')
    .post(externalGroup);

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ffd0e118d33cf4b4a000eb4f96895ecf45aea392632578129972f315f5ffc10
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278385"
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
    .version('beta')
    .post(externalGroup);

```
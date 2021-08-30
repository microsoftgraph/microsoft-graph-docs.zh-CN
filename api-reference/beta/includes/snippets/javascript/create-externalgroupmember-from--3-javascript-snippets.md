---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a3fd37440cd82c0726332514593014cdf858b2541c5f839fd5dac5ee73af010
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161871"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalGroupMember = {
  id: '1431b9c38ee647f6a',
  type: 'group',
  identitySource: 'external'
};

await client.api('/external/connections/contosohr/groups/31bea3d537902000/members')
    .version('beta')
    .post(externalGroupMember);

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a641a40702b166487047fad036ab1695e6786a7c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102028"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalGroupMember = {
  id: 'e811976d-83df-4cbd-8b9b-5215b18aa874',
  type: 'user',
};

await client.api('/external/connections/contosohr/groups/31bea3d537902000/members')
    .version('beta')
    .post(externalGroupMember);

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f7a9d7b51fe8f8096625ea2a47550ac57188187
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022640"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identity = {
  id: 'e811976d-83df-4cbd-8b9b-5215b18aa874',
  type: 'user'
};

await client.api('/external/connections/contosohr/groups/31bea3d537902000/members')
    .post(identity);

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1f4f5a6361ed4ad1bdacfc3e3f8489e7d4061e8
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210037"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const teamworkTag = {
  displayName: 'Finance',
  members: [
    {
        userId: '92f6952f-61ca-4a94-8910-508a240bc167'
    },
    {
        userId: '085d800c-b86b-4bfc-a857-9371ad1caf29'
    }
  ]
};

await client.api('/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags')
    .version('beta')
    .post(teamworkTag);

```
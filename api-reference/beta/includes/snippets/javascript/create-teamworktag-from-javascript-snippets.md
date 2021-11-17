---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3de9bdb7e14758209349053c68bfde297dff81715a9ea3d301011e53257b47a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162853"
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
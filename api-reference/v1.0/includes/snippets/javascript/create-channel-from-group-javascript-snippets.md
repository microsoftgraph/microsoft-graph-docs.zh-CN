---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8627aa3dc6068cb5e7bc2e640953628f9b620bbe
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508452"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const channel = {
  displayName: 'Architecture Discussion',
  description: 'This channel is where we debate all future architecture plans',
  membershipType: 'standard'
};

await client.api('/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels')
    .post(channel);

```
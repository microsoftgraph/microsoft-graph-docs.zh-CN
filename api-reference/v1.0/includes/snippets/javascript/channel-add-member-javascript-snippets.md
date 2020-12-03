---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24df8a9cbe73e47edb5fd19456c0f0d765e1051f
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523312"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19:56eb04e133944cf69e603c5dac2d292e@thread.skype/members')
    .post();

```
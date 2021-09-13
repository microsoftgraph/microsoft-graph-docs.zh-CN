---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9fc6da4001ef871396ddbb96a4130ce7a7cefe4182049cd5f8ba0b47ee745ca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902326"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const muteParticipantOperation = {
  clientContext: 'clientContext-value'
};

await client.api('/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/mute')
    .post(muteParticipantOperation);

```
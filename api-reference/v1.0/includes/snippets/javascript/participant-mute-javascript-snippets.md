---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19275c628a20f50301b49c4e39af9b2a4e1ccb31a146686d87c06e2c794a2fce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332969"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const muteParticipantOperation = {
  clientContext: 'd45324c1-fcb5-430a-902c-f20af696537c'
};

await client.api('/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/participants/2765eb15-01f8-47c6-b12b-c32111a4a86f/mute')
    .post(muteParticipantOperation);

```
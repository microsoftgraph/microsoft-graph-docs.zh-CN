---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c465355dd6611a95ae762af71f526a7a584f14e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949994"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const teamsTab = {
  displayName: 'My Contoso Tab - updated again'
};

await client.api('/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs/794f0e4e-4d10-4bb5-9079-3a465a629eff')
    .update(teamsTab);

```
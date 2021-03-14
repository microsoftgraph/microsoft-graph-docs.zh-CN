---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22b2cdcab8cd0d574243055547d449257aa36003
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804020"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chatMessage = {
  body: {
    contentType: 'html',
    content: 'Hello World'
  }
};

await client.api('/teams/{id}/channels/{id}/messages/{id}/replies')
    .post(chatMessage);

```
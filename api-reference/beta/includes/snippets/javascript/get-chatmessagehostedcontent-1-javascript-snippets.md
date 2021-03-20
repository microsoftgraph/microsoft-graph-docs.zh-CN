---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da3133690247fddf59a84504024be10ca0ea29ce
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947746"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let chatMessageHostedContent = await client.api('/chats/{id}/messages/{id}/hostedContents/{id}')
    .version('beta')
    .get();

```
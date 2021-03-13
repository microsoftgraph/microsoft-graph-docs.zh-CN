---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1b2028fe909ad3ac63d92d1235c7438c742be5d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799974"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  '@odata.type': '#microsoft.graph.fileAttachment',
  name: 'smile',
  contentBytes: 'a0b1c76de9f7='
};

await client.api('/me/messages/AAMkpsDRVK/attachments')
    .version('beta')
    .post(attachment);

```
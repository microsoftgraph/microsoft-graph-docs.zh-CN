---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b88476130efcc0cb614080b721fa03e2b711d70b4d15fa4bfe33edba5072518b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106639"
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
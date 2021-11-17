---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0aca1fb8e4b180e55f34675f5a73b6ca767fc158ce0ca6dd328fc13be35662a1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104532"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const uploadSession = {
  AttachmentItem: {
    attachmentType: 'file',
    name: 'flower', 
    size: 3483322
  }
};

await client.api('/me/messages/AAMkADI5MAAIT3drCAAA=/attachments/createUploadSession')
    .version('beta')
    .post(uploadSession);

```
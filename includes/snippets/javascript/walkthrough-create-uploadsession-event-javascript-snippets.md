---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 036521711548198ed807e9ad39d78da5cc41c450
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567382"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const uploadSession = {
  AttachmentItem: {
    attachmentType: "file",
    name: "flower",
    size: 3483322
  }
};

let res = await client.api('/me/events/AAMkADU5CCmSAAA=/attachments/createUploadSession')
    .post(uploadSession);

```
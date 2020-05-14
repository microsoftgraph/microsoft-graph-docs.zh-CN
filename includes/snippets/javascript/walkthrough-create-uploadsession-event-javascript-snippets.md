---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd22fd1ab0434c92af573833a2ad738462433746
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44052430"
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
    .version('beta')
    .post(uploadSession);

```
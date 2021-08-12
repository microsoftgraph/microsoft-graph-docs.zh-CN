---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fff75694d500c025e294ef0f0a8c39272bf743213376d29c45e56e5ad7bb275
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54240408"
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
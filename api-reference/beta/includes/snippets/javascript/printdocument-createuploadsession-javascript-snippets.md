---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af48c5ea690839044e49a363658750dbe70d0982
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921852"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const uploadSession = {
  properties: {
    documentName: 'TestFile.pdf',
    contentType: 'application/pdf', 
    size: 4533322
  }
};

await client.api('/print/shares/1c879027-5120-4aaf-954a-ebfd509a3bcc/jobs/46207/documents/9001bcd9-e36a-4f51-bfc6-140c3ad7f9f7/createUploadSession')
    .version('beta')
    .post(uploadSession);

```
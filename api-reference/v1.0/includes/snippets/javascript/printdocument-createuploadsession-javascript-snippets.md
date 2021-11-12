---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a2dcb3d98f752959cf6cefd9b3eafc4a38208a6cceb53dbbeab7aa69484bf13
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158425"
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

await client.api('/print/printers/{printerId}/jobs/{printJobId}/documents/{printDocumentId}/createUploadSession')
    .post(uploadSession);

```
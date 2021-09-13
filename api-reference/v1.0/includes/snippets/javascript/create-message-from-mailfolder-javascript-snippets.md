---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1d9ff53216e7d7c09fab3d1467d070a2abcbbf5e967cc956d0713fa647d3194
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332040"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  receivedDateTime: 'datetime-value',
  sentDateTime: 'datetime-value',
  hasAttachments: true,
  subject: 'subject-value',
  body: {
    contentType: '',
    content: 'content-value'
  },
  bodyPreview: 'bodyPreview-value'
};

await client.api('/me/mailFolders/{id}/messages')
    .post(message);

```
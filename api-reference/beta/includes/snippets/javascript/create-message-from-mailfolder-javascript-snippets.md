---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dadf4e816d696c3ea508360ca8de0e52309bab707b999e61793e4fee4ba7bb91
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164328"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  receivedDateTime: '2016-10-19T10:37:00Z',
  sentDateTime: '2016-10-19T10:37:00Z',
  hasAttachments: true,
  subject: 'subject-value',
  body: {
    contentType: '',
    content: 'content-value'
  },
  bodyPreview: 'bodyPreview-value'
};

await client.api('/me/mailFolders/{id}/messages')
    .version('beta')
    .post(message);

```
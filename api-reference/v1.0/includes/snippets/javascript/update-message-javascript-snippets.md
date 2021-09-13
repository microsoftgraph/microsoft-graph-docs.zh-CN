---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8173e5dd90b97e42d05e8f9fdbeb585ebb02f0c4eb94f7c682a56c2f9df1811
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56831192"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  subject: 'subject-value',
  body: {
    contentType: '',
    content: 'content-value'
  },
  inferenceClassification: 'other'
};

await client.api('/me/messages/{id}')
    .update(message);

```
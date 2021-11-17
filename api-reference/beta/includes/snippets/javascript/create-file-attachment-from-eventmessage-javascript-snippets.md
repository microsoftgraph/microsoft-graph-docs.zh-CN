---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 336be4d9f9d27dde1c89455f7ee17a3be6caf61ec527b44d73d80daae64afd9e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215850"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  '@odata.type': '#Microsoft.OutlookServices.FileAttachment',
  name: 'name-value',
  contentType: 'contentType-value',
  isInline: false,
  contentLocation: 'contentLocation-value',
  contentBytes: 'contentBytes-value'
};

await client.api('/me/messages/{id}/attachments')
    .version('beta')
    .post(attachment);

```
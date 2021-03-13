---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5804193f82d2a520b56cd6cef2c979471e10c58
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781845"
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
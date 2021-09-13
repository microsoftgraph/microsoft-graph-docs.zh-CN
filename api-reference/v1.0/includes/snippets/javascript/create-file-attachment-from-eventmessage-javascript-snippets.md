---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2cc08139462ed99417adfbba025cd2108b75e855c16cc99a4007003bf5bea30b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903333"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  '@odata.type': 'microsoft.graph.fileAttachment',
  name: 'name-value',
  contentType: 'contentType-value',
  isInline: false,
  contentLocation: 'contentLocation-value',
  contentBytes: 'base64-contentBytes-value'
};

await client.api('/me/messages/{id}/attachments')
    .post(attachment);

```
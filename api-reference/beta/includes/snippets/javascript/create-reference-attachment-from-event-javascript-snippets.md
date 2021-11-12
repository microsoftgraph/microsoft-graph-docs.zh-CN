---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d05119cf2aec46df4a5330844370718130319f6940027c726144a54fd3698708
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902503"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
    '@odata.type': '#microsoft.graph.referenceAttachment',
    name: 'Personal pictures',
    sourceUrl: 'https://contoso.com/personal/mario_contoso_net/Documents/Pics',
    providerType: 'oneDriveConsumer',
    permission: 'Edit',
    isFolder: 'True'
};

await client.api('/me/events/AAMkAGE1M88AADUv0uAAAG=/attachments')
    .version('beta')
    .post(attachment);

```
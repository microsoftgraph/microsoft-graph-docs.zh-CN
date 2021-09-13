---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 507ec24c26e639de971501e8dadff9b4848c293bc8661b131caa8ae1b0227ac9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903334"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  '@odata.type': '#Microsoft.OutlookServices.ItemAttachment',
  name: 'name-value',
  item: {
    '@odata.type': 'microsoft.graph.message'
  }
};

await client.api('/me/events/{id}/attachments')
    .post(attachment);

```
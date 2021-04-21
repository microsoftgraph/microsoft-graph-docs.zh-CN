---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86ddafad5f70eb18ad644dee9dfbecea5fe7877f
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921144"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printerShare = {
  name: 'name-value',
  'printer@odata.bind': 'https://graph.microsoft.com/beta/print/printers/{id}'
};

await client.api('/print/shares')
    .version('beta')
    .post(printerShare);

```
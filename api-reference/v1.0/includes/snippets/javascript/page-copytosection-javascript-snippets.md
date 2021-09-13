---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1651d83662842ec2828bcc7624a39005326d55d5a7cd53b940554338af38e04
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220548"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteOperation = {
  id: 'id-value',
  groupId: 'groupId-value'
};

await client.api('/me/onenote/pages/{id}/copyToSection')
    .post(onenoteOperation);

```
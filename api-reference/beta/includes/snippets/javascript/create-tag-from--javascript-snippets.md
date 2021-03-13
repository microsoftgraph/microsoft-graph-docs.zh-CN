---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25799816168b76efe79c5a1233123c7164ebbc79
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773765"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tag = {
  displayName: 'Privileged',
  description: 'The document is privileged',
  'parent@odata.bind':'https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/98fdad78bbce4519b75474bc150575c3'
};

await client.api('/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags')
    .version('beta')
    .post(tag);

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e578d9721fe037b564dfcb714c3fccce9ed887de5907092040cdce9a1d241e16
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161507"
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
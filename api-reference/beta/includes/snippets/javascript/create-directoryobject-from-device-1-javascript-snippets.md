---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12d5ea21a6b62640a41c5b7a2cb80220b212956730e023e77ae5a914edc01fac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332520"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id': 'https://graph.microsoft.com/beta/directoryObjects/{id}'
};

await client.api('/devices/{id}/registeredOwners/$ref')
    .version('beta')
    .post(directoryObject);

```
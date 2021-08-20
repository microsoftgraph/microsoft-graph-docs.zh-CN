---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc353a439c4de03428d157fa0258c21ec2e791aa0d0d9e31761f7ab98e4345ba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107030"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id': 'https://graph.microsoft.com/v1.0/directoryObjects/{id}'
};

await client.api('/groups/{group-id}/members/$ref')
    .post(directoryObject);

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a219b7f6986dd5f339ec6bd9c869bcd30eb6285295125e848c892863ebe996b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902989"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id': 'https://graph.microsoft.com/v1.0/directoryObjects/{id}'
};

await client.api('/devices/{id}/registeredOwners/$ref')
    .post(directoryObject);

```
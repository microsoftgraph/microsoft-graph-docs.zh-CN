---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca55f2754f0ea68ebd2cf78cdee1c8a1735f3ef70ce19d6c61c1098cb01d89ce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277977"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let set = await client.api('/sites/microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f/termStore/sets/8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f')
    .version('beta')
    .get();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec8d7bf9eea7d5aac95c1a955cb8a2c254760e49c895eb300220f73ad5cc8484
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278461"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let itemPhone = await client.api('/me/profile/phones/{id}')
    .version('beta')
    .get();

```
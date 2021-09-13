---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: abf54c15bdcc5fbf5004f19824f9c84ef6ddb50905274846b5be0f4875c1bc9f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163473"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sharedDriveItem = await client.api('/shares/{shareIdOrEncodedSharingUrl}')
    .get();

```
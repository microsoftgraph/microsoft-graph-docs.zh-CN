---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9d8bcdefa703fcc2fdba7fc71d772cf24fa0ab5db30a4b6cea2992a38be02ac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106195"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let driveItem = await client.api('/drive/items/{bundle-id}?expand=children')
    .version('beta')
    .get();

```
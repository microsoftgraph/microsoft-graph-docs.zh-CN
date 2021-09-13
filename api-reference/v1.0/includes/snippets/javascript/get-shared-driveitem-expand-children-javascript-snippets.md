---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03c3d7b5e502a7e6eb381d1a6a766f3a6496b1f9dd7a3801ca53b0a142fab38c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218663"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let driveItem = await client.api('/shares/{shareIdOrUrl}/driveItem')
    .expand('children')
    .get();

```
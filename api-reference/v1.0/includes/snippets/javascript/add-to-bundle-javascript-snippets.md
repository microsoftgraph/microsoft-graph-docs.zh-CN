---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ed3f52cec4f05e789ed248bc23095afd4afd453
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758265"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  id: '123456!87'
};

await client.api('/drive/bundles/{bundle-id}/children')
    .post(driveItem);

```
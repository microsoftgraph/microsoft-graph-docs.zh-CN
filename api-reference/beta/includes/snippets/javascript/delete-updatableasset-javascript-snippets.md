---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7746012c438a733a933e228b2d38a29ed6b05be20875204b4aa0f118b328bd29
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158440"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/admin/windows/updates/updatableAssets/{updatableAssetId}')
    .version('beta')
    .delete();

```
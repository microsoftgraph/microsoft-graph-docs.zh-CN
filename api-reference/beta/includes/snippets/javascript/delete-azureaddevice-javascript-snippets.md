---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef0ac8e37a30b4d636263cfb7bdd5530e78b17b532608d409a730228db873f81
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163589"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/admin/windows/updates/updatableAssets/{azureADDeviceId}')
    .version('beta')
    .delete();

```
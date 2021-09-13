---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf61116ea144eed483063c580e3785aec30d0ef97bf531b0c9e3ed42c246dc42
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903715"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/{user-id}')
    .delete();

```
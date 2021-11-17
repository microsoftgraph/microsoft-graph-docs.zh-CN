---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d0f42f04ca4b97c7f67470cc9c2b86bc55428ee13b9723d8adb0f8edbe7d7c4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333133"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/synchronizationProfiles/{id}/resume')
    .version('beta')
    .post();

```
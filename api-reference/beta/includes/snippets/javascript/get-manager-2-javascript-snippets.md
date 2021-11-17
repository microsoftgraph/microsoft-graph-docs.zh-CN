---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d50c753b7a7f2cd1a97caa273bc42e80d43cba88a9e088fa792881c0e34282f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378561"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryObject = await client.api('/users/{id|userPrincipalName}/manager')
    .version('beta')
    .get();

```
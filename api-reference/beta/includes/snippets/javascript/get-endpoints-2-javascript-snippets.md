---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eba4b9113d0ad8ae0e1a551ee8e8d0c4163aaba3cfbe5752860064ff7259dded
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904237"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let endpoints = await client.api('/print/services/{id}/endpoints')
    .version('beta')
    .get();

```
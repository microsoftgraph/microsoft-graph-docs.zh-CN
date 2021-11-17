---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1906730dd1eb06d09618f5e59112c5840fcdf7cbe9a097e4b6e6459ddb2a375
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105215"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drive = await client.api('/me/drive')
    .version('beta')
    .get();

```
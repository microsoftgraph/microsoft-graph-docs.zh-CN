---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65c909dea8a463d9a7335458f7bd09f83f65de0850fa0212c6da796629c99ac7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219041"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let photos = await client.api('/groups/{id}/photos')
    .version('beta')
    .get();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5816dc2112811a2fa9962e3d6866eb42801f5cf1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800659"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const languageProficiency = {
  displayName: 'Norwegian Bokmål',
  tag: 'nb-NO',
  spoken: 'nativeOrBilingual',
  written: 'nativeOrBilingual',
  reading: 'nativeOrBilingual'
};

await client.api('/me/profile/languages')
    .version('beta')
    .post(languageProficiency);

```
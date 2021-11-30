---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95dab8ea74fe7420a43703395de9cbd083b1ce55
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61223545"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attributeSet = {
    description: 'Attributes for engineering team',
    maxAttributesPerSet: 20
};

await client.api('/directory/attributeSets/Engineering')
    .version('beta')
    .update(attributeSet);

```
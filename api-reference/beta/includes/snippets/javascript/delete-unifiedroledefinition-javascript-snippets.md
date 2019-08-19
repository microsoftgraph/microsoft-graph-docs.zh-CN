---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 170cfaea7ecb91237024705b0f094f9f2fc38802
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461587"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a')
    .version('beta')
    .delete();

```
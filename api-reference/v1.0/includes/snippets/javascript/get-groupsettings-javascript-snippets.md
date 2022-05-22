---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21b2d57d2dfff4982b14cf4db42660a69909c9b9
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629803"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groupSetting = await client.api('/groups/05aa6a98-956a-45c0-b13b-88076a23f2cd/settings/a06fa228-3042-4662-bd09-33e298da1afe')
    .get();

```
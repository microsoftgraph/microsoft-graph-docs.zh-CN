---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3ca645b685571e851434f105edd29b7a8b6ace3
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48462555"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07')
    .delete();

```
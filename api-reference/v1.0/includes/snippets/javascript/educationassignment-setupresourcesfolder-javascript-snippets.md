---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29451e659125edfa28ec530dfcd1e062d8fd439a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59020065"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationAssignment = {
};

await client.api('/education/classes/955e0bd5-52c2-41ad-b7e8-5b33a18c5e78/assignments/18d17255-3278-49fb-8da7-d095b7f610c4/setUpResourcesFolder')
    .post(educationAssignment);

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45a33bc412c7f3a3ed5c194eee509383c4b081c0
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336737"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let group = await client.api('/sites/mycompany.sharepoint.com,8f03a01c-dcfa-4aaf-9be5-b3fb48e538c1,739084f3-c0fa-46ac-b7f8-13b344781ad0/termStore/groups/1FFD3F87-9464-488A-A0EC-8FB90911182C')
    .get();

```
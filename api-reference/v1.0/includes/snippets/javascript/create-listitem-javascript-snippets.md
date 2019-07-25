---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f580373ff0b76c33ee5bcb4e360a236de2703807
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731604"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const listItem = {
  fields: {
    Title: "Widget",
    Color: "Purple",
    Weight: 32
  }
};

let res = await client.api('/sites/{site-id}/lists/{list-id}/items')
    .post({listItem : listItem});

```
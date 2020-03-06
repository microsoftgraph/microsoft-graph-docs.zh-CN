---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8db8095b4123f542e4a538259746eb4c62cd37de
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636825"
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
    .post(listItem);

```
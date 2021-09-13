---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a8ed85bd2f13ac10b1c2c46ab0d3e1226f5c9bd077543d7e2203c2f24673adb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333769"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/sites/{site-id}/lists/{list-id}/items/{item-id}')
    .delete();

```
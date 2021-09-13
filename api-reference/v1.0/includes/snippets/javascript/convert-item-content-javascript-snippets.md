---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08f00640f579bb9dba64f74fb54448314b257042fdad46a980903b907f9737d2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104601"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/me/drive/items/{item-id}/content?format=%7Bformat%7D')
    .get();

```
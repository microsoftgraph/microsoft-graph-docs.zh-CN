---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e87120ce797cbcfb7397cab449f059336075eabbcf9e85fc61714e3f6ef61640
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333508"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let classes = await client.api('/education/me/classes')
    .get();

```
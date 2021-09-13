---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5fc28f64fb03a370fa5b1090901054468de1558dd254d155a1455b78db50db52
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162598"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teachers = await client.api('/education/classes/{class-id}/teachers')
    .get();

```
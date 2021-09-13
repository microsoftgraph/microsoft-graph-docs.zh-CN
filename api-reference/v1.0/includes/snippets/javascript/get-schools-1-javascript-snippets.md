---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4339e313fb7b9073ee695b1c50ca92d6b504bfdbe26558e4b50c81a708a95dad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101337"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schools = await client.api('/education/classes/{class-id}/schools')
    .get();

```
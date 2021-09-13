---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d54ab8d0127eb09f25c73242de566bd7792d346bd76dbce8d2856eb49a78d72f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409573"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  '@odata.id':'https://graph.microsoft.com/v1.0/education/users/14011'
};

await client.api('/education/classes/{class-id}/teachers/$ref')
    .post(educationUser);

```
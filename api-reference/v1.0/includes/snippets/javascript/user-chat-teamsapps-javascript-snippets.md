---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db13198e985f06132dd999e1e23e25be948d255f63141113e32d0cae83c3d007
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279297"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let chat = await client.api('/users/f32b83bb-4fc8-4db7-b7f5-76cdbbb8aa1c/teamwork/installedApps/ZjMyYjgzYmItNGZjOC00ZGI3LWI3ZjUtNzZjZGJiYjhhYTFjIyMyMmY3M2JiZS1mNjdhLTRkZWEtYmQ1NC01NGNhYzcxOGNiMmI=/chat')
    .version('beta')
    .get();

```
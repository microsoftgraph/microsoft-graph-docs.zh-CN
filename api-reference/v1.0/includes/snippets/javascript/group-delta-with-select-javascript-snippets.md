---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd87017d8cef23a6f20cb9dfed45deae969d9adbb7cc0ce69cbfb2fc9f51a2f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332590"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/groups/delta')
    .select('displayName,description,mailNickname')
    .get();

```
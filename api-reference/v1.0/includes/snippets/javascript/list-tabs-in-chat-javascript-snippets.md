---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea76253442bebee8abe7444474a303b256a5cd61ff48394b70ab8b7d2b41df28
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904157"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tabs = await client.api('/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs')
    .expand('teamsApp')
    .get();

```
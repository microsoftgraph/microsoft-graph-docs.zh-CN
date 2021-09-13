---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bcabf811383c441cb082673165f4ea111e84f7914cd1841ed7abe1d3a711aca5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106717"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messageRule = await client.api('/me/mailFolders/inbox/messageRules/AQAAAJ5dZqA=')
    .get();

```
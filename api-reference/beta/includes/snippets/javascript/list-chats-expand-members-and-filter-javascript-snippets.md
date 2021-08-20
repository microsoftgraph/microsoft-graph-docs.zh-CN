---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01052a9944c866f31fc1d5bee5dfa2dfc4cc9812ce691fdabcab8b5f81d076ae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162513"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let chats = await client.api('/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats')
    .version('beta')
    .filter('members/any(o: o/displayname eq \'Peter Parker\')')
    .expand('members')
    .get();

```
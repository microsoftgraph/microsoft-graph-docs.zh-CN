---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc2a496f90ff00718327d7b4be9941cc2375fdb5806b124c7fa0dff2dc0dd21c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902293"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let replies = await client.api('/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616989510408/replies')
    .get();

```
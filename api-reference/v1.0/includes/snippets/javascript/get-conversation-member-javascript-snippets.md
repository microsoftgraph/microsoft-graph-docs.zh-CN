---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 585a03243cd4fd0d4ea9953fcb3276f8439a5055
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954851"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conversationMember = await client.api('/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/141c574c-dd90-4131-b173-baf4bb0e894e')
    .get();

```
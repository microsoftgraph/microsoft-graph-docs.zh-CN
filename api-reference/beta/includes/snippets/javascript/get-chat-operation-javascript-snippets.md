---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: baa2032f43285617f9e1ef6790063465eb3ac09ca06170774826f050b331eb1b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328987"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsAsyncOperation = await client.api('/chats/19:c253a29b5f694b55a6baad8e83510af7@thread.v2/operations/2432b57b-0abd-43db-aa7b-16eadd115d34-e88ae9aa-887e-4972-ac3e-bd578e38232e-cf58835e-43f0-4fc1-825e-5de55630e7e4')
    .version('beta')
    .get();

```
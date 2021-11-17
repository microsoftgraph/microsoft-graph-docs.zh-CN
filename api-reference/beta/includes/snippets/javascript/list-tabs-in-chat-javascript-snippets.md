---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08147d8d4f4cd58d0eb2571a981a53b2117b756c6c7dccaf7b9265c0d98d3248
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219782"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tabs = await client.api('/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs')
    .version('beta')
    .expand('teamsApp')
    .get();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4bb8b8c615f81dd8a30ab8c75195b3f8908438bb6ab9a21d0f68914b19583a6b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903325"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let acceptedSenders = await client.api('/groups/{id}/acceptedSenders')
    .get();

```
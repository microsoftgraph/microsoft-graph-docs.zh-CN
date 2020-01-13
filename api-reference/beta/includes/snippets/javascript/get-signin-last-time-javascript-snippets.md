---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 551fe9b4c6180fef448902b7e20ec7f22b11c878
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37996309"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users')
    .version('beta')
    .select('displayName,userPrincipalName')
    .get();

```
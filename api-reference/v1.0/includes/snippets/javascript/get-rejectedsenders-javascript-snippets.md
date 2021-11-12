---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9297247c4521b51684398fdb347cd0d5a27049fa3a18ac2c630cd617b82f76f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104576"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let rejectedSenders = await client.api('/groups/{id}/rejectedSenders')
    .get();

```
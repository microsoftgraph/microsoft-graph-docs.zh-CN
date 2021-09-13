---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a4845c921b380b361f75099cfb41a83d77a156a5151d6525a2ff06d286e4d61
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277373"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{id}/unarchive')
    .post();

```
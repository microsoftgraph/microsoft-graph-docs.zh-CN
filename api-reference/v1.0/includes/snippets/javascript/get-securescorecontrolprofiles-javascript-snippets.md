---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 188d41fda823d658283f3614fd52586d722c514e01f4f71a9c5b0ffe07aa7b5e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334088"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let secureScoreControlProfiles = await client.api('/security/secureScoreControlProfiles')
    .get();

```
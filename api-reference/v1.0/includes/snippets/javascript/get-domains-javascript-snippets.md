---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a88766c79dda08f173bdf3ad401756ef01fe01f4803f09a3003515794eb6f617
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107070"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let domains = await client.api('/domains')
    .get();

```
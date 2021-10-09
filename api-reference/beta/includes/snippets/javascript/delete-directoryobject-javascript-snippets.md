---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 175f9b22d1f9c3b609f13cb921a4ef50d6ccf1903f99e81501c58570a4144d31
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106554"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/directoryObjects/ffab4dce-9b82-49a6-b7c7-1a143106598c')
    .version('beta')
    .delete();

```
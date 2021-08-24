---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9ddded9117e50a8905ed6e97f7961b8ee510273806d09cefbd9ee9106ee2848
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903812"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directorySettingTemplates = await client.api('/directorySettingTemplates')
    .version('beta')
    .get();

```
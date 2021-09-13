---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e72ed3edd6238c33e28557b36cc4cad95453e130c71627aace413773586dbf8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904305"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/messages/{id}/send')
    .post();

```
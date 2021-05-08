---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a570c3cd4bd88e7d8fcf4047a7b57c27a44c1a8
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240943"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let noncustodialDataSource = await client.api('/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/noncustodialDataSources/8b69818bf6af4f8a9dede428401c71e7')
    .version('beta')
    .get();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b45084c5d72bdac98524b2cc74d4f143712c06461c4ed70a6335fa1a8e7b285d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158376"
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
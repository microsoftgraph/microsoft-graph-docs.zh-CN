---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b7c902d6f308487101aaa7adaf33c6d9b15bac5c1240a38fbc4d802e09c6d47
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278392"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let custodianSources = await client.api('/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/custodianSources')
    .version('beta')
    .get();

```
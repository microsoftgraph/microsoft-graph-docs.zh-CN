---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b1b5fee136b1b4a2b7cf7b59356bcc6c441fb611d0c5352562d3863ee6db2b04
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164295"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let serviceConfigurationRecords = await client.api('/domains/{domain-name}/serviceConfigurationRecords')
    .get();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b36ede139e0497a759aaf88d554ff59f0881ca3
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994807"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/connections/contosohr/operations/3ed1595a-4bae-43c2-acda-ef973e581323')
    .version('beta')
    .get();

```
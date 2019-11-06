---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a1925214fce8604ecae40096a29e8ef92528d12
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996129"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/range')
    .version('beta')
    .get();

```
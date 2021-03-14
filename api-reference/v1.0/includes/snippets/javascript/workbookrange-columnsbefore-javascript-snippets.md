---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76a8d469b1091d114a51443afb3a8114b10b4d57
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782254"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=2)')
    .get();

```
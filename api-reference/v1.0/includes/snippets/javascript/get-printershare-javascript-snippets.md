---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97f013ec9f0ae6350260635ad393d7d0dcaa321bf9bc076cfa950b993a80a79d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333759"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printerShare = await client.api('/print/shares/{printerShareId}')
    .get();

```
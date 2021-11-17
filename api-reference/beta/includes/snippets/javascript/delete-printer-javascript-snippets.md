---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb1045fc7f8e4d33cb6be59bd1f01e55380dbf359c34160029ab750f2aa2dabc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902394"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/printers/{id}')
    .version('beta')
    .delete();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4891c2bfd815171ad29ba034d2a60b3aa9f91acb7387b6d8be34c40bc5a9f7a9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104761"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printJob = await client.api('/print/printers/86b6d420-7e6b-4797-a05c-af4e56cd81bd/jobs/31216')
    .version('beta')
    .expand('documents')
    .get();

```
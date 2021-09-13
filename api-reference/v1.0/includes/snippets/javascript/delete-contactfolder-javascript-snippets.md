---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b0d14cba8447c5e9ea58463b9f0fbd096bfe85d4b5d5af996968bd28642d86e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105407"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/contactFolders/{id}')
    .delete();

```
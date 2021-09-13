---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3dc37467bd426f4559007f1a2e08e4da9dea98cc6df6ff809a2050dabcf8169
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101334"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const forceDelete = {
  disableUserAccounts: true
};

await client.api('/domains/{id}/forceDelete')
    .post(forceDelete);

```
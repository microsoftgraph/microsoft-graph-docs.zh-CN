---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29a6f2c19084d8a69ca8269fe070897fc50368ef14a4346ec2067e230f607626
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161328"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8')
    .delete();

```
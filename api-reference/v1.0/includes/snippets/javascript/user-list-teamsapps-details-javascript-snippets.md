---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 495dce763abd88dbe3331abcbed83588fcc9e72c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788126"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let installedApps = await client.api('/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps')
    .expand('teamsAppDefinition')
    .get();

```
---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cffb4de13f2c331739d82af6cfd53660a0261eda5fa7efca0f78d3ded8b32a6c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215946"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members')
    .get();

```
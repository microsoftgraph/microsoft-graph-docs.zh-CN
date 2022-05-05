---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21976769d8e9843246e922917a74d54909cc576d
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220265"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/directoryObjects/ffab4dce-9b82-49a6-b7c7-1a143106598c')
    .delete();

```
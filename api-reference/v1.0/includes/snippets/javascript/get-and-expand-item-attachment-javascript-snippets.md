---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d92cffb05067233d554d39fbe7cb90e4518256302f69756ef5e3931524dcf49c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903566"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let attachment = await client.api('/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=/')
    .expand('itemattachment/item')
    .get();

```
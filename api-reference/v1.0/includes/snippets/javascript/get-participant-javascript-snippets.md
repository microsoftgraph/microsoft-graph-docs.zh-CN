---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52a421be04470e1a9f3cc596a673d1af0287341a05f20b604b95165cabbf8d9c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221397"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let participant = await client.api('/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants/7e1b4346-85a6-4bdd-abe3-d11c5d420efe')
    .get();

```